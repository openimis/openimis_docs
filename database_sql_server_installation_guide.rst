
Database installation guide (SQL Server)
========================================

Install SQL Server
------------------

Note: This installation guide is based on SQL Server 2017.

Download the desired version of SQL Server (for example, the Express version from https://www.microsoft.com/en-us/sql-server/sql-server-downloads).

Open the setup file. Select New Installation or add feature to an existing installation.

On the Features selection:

- In Shared Feature section, select SQL Client Connectivity SDK
- For installations with Data Warehouse, select Analysis Services, Reporting Services and Integration Services (not available for the Express edition)

On the Instance configuration, the default name (SQLEXPRESS) can be used, unless it is already used by another instance.

On Database engine configuration, select Mixed Mode (SQL Server authentication and Windows authentication) in Authentication Mode.

Continue the setup process until the installation is complete.

Configure SQL Server
--------------------

Open the SQL Server Configuration Manager

- On the left panel, select SQL Server Network Configuration → Protocols for SQLEXPRESS (or the name of your SQL Server instance)

  - Enable Named Pipes and TCP/IP

- Select SQL Server Services

	- Right click on SQL server (instance name) and select Restart

Initialise SQL Server database
------------------------------

To facilitate the setting up of the openIMIS database, it is suggested to install `SQL Server Management Studio<https://docs.microsoft.com/sql/ssms/download-sql-server-management-studio-ssms>` (SSMS). The following procedure is based on SSMS, but you can use the standard SQL Server prompt to proceed with the setup.

First, download the openIMIS database backup files and migration scripts from Github repository (the source code ZIP file).

In SQL Server Management Studio:

- Restore the initial database provided in the release sources. Choose the database to restore based on your context. There are 3 types of databases (structurally identical, but they are pre-configured differently):

    - Online: this is the default choice when deploying a central online server
    - Offline: this mode is sometime used for remote insurance offices without connectivity. Note: the synchronisation of data with the central server is manual.
    - Offline HF: this database can be used in remote health facilities without connectivity. Note: the synchronisation of data with the central server is manual.

- In the Object Explorer: openIMIS (the openIMIS db name) → Programmability → Stored Procedures → dbo.SETUP-IMIS
- Right click on the dbo.SETUP-IMIS and execute the procedure. The result returned from the procedure should be 0.

Create a dedicated user with full privilege on the openIMIS database only:

- In the Security → Logins → right click and select “New Login…”
- In General page:

    - Give a login name (i.e. ImisUser)
    - Select SQL Server authentication and provide a password
    - Unselect Enforce password expiration
    - Change default database to openIMIS

- In User Mapping page:

    - Map IMIS db to ImisUser user
    - Give the role of db_owner

Upgrade the openIMIS database
-----------------------------

If an existing openIMIS database exists already, follow the next steps to upgrade it to the desired version:

- Download the openIMIS database backup files and migration scripts from `Github repository <https://github.com/openimis/database_ms_sqlserver/releases/latest>` (the source code ZIP file).
- In SQL Server Management Studio, run the migration script on the openIMIS database.
