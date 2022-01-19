


User roles/profiles
^^^^^^^^^^^^^^^^^^^

  IMIS uses the concept of user profiles (roles) that can be associated with users. Some roles are predefined and they are designated as system roles. Their purpose is guarantee compatibility with the previous versions of IMIS.
  
  User roles/profiles administration is restricted to users with the role of openIMIS Administrator.

  
Navigation
""""""""""

  All functionality for use with the administration of user roles can be found under the main menu ``Administration``, sub menu ``Users Profile``.

  .. _register_nav_user_roles:
  .. figure:: /img/user_manual/register_nav_user_roles.png
    :align: center

    `Image - Navigation User Roles/profiles`

  Clicking on the sub menu ``Users`` re-directs the current user to the `User roles/profiles control page <#user-roles-profiles-control-page>`__\ .

  .. _user_roles_control_page:
  .. figure:: /img/user_manual/user_roles_control_page.png
    :align: center

    `Image - User roles/profile control page`

User roles/profiles control page
"""""""""""""""""""""""""""""""""

The ``User roles/profile control page`` is the central point for all user roles/profiles administration. By having access to this page, it is possible to add, edit, delete and search users roles/profiles. The page is divided into four panels (:ref:`Image User roles/profiles control page<user_roles_control_page>`).

Administration of users’ profile s(roles) is not included in any system role. It can be accomplished by the Admin user or by users to which such administration is delegated (by defining a role including an access to Administration/User Profiles) by the Admin user.

    **Pre-conditions**

      A new user profile may only be added or thereafter edited, after an approval of the management of the scheme administration. It can be accomplished at the beginning only by the Admin user. The Admin user can define a new user profile incorporating also adding, editing  or deleting of  user profiles and create new users  with this profile. In this way, rights to the register of user profiles can be delegated to other users besides the Admin user.

    **Navigation**

      All functionality for use with the administration of user profiles can be found under the main menu ADMINISTRATION, sub menu USER PROFILES

 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. The following search options are available which can be used alone or in combination with each other.

    Role Name
      When set the search will display the roles with a name that start with the content of the filter , `%` can be used as a wildcard meaning a search with `%er` will display all the result containing `er` in the name 

    System
      The system user profiles match the previous roles for compatibility reasons.
      When set to `TRUE` the search will display the default roles, 
      when set to `FALSE` the search will display only the custom roles

    Blocked
      The blocked user profiles are temporarily not acting in the sense that their access rights are not available to users to whom blocked user profiles were assigned.
      When set to `TRUE` the search will display the roles that were blocked, 
      when set to `FALSE` the search will display only the unblocked roles

    Historical
      Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records 
      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records (:ref:`User roles results <user_roles_result>`).


 #. **Result Panel**


    The Result Panel displays a list of all roles/profiles found, matching the selected criteria in the Search Panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image User roles results panel<user_roles_result>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the `Change user role/profile Page <#user-role-profile-page>`__.
    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel

    .. _user_roles_result:
    .. figure:: /img/user_manual/user_roles_result.png
      :align: center

      `User roles results panel`

    * Blue background: Selected record
    * Yellow background: hovered records
    * Strikethrough: historical records

    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:ref:`Image User roles/profile control page<user_roles_control_page>`)

 #. **Button Panel**

    * The ``Add`` button will `add a new role/profile <#adding-a-user-role-profile>`__ (not available if ``Historical`` was checked)
    * The ``Edit`` button will `edit a role/profile <#editing-a-user-role-profile>`__. not available if ``Historical`` was checked)
    * The ``Duplicate`` bbutton will `duplicate a role/profile <#duplicating-a-user-role-profile>`__ (not available if ``Historical`` was checked)
    * The ``Delete`` button will `deleting a role/profile <#addeleting-a-user-role-profile>`__ (not available if ``Historical`` was checked)
    * The ``Cancel`` button re-directs to the :ref:`Home Page <home_page>`.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a user role/profile has been added, updated or deleted or if there was an error at any time during the process of these actions.

User role/profile Page
""""""""""""""""""""""

    .. _user_role_page:
    .. figure:: /img/user_manual/user_role_page.png
      :align: center

      `Image - User role/profile page`

 #. **Data Entry - Role details**


    Role Name
      Enter the name of the role/profile, this name will be used as reference in the `User roles/profiels control page <#user-roles-profiles-control-page>`__ and `Users page <#user-page>`__

    Alternative language
      Translation of the role name for the second language of openIMIS

    System
      Read-only checkbox indicating whether the user profile is a system one or not.

    Blocked
      If checked the user profile is blocked

 #. **Data Entry - Rights details**

    Insurees and Policies
      list of the right available for the `Insurees and Policies` module:

        * CRUD rights (Create, read/search, update/edit and Delete):

          - Family/Group

          - Insuree

          - Policy

          - Contribution

        * Business specific roles

          - Renew policy

          - Enquire insuree

    Claims
      list of the right available for the `Claims` module:

        * CRUD rights (Create, read/search, update/edit and Delete):

          - Claims

        * Business specific roles:

          - Claims:

            - Print

            - Submit

            - Review

            - Feedback

            - Update

            - Process

          - Claim Batch:

            - Process

            - Filter

            - Preview


    Administration
      list of the right available for the `Administration` module:

        * CRUD rights (Create, read/search, update/edit and Delete):

          - Products

          - Health Facilities

          - Pricelists – Medical Services

          - Pricelists – Medical Items

          - Medical Services

          - Medical Items

          - Enrolment Officers

          - Claim Administrators

          - Users

          - User roles/profiles

          - Payers

          - Locations

        * Business specific roles

          - Duplicate Products

          - Duplicate Pricelists – Medical Services

          - Duplicate Pricelists – Medical Items

          - Duplicate User roles/profiles

          - Move Locations

    Tools
      list of the business rights available for the `Tools` module

        * Register

          - Upload Diagnoses

          - Upload Health Facilities

          - Upload Locations

          - Download Diagnoses

          - Download Health Facilities

          - Download Locations

        * Extracts

          - Download Mater-data

          - Create Phone Extracts

          - Create Offline Extract

          - Upload Claims

          - Upload Enrolments

          - Upload Feedback

        * Run report

          - Primary Operational Indicators-policies

          - Primary Operational Indicators-claims

          - Derived Operational Indicators

          - Contribution Collection

          - Product Sales

          - Contribution Distribution

          - User Activity Report

          - Enrolment Performance Indicators

          - Status of Registers

          - Insurees without Photos

          - Payment Category Overview

          - Matching Funds

          - Claim Overview

          - Percentage of Referrals

          - Families and insurees Overview

          - Pending Insurees

          - Renewals

          - Capitation Payment

          - Rejected Photos

        * Utilities/Email setting

          - Backup

          - Restore

          - Execute Script

          - Email Setting

 #. **Buttons**

    Save
      Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `User Control Page <#user-control-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the user has been saved will appear on the Information Panel.

    Cancel
      By clicking on the ``Cancel`` button, the user will be re-directed to the `User roles/profiles control page. <#user-roles-profiles-control-page>`__

    **Mandatory data**

      If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data fields will take the focus (by an asterisk on the right of the corresponding data field).

Adding a User role/profile
""""""""""""""""""""""""""

  Click on the Add button to re-direct to the  `User role/profile Page <#user-role-profile-page>`__.

  When the page opens all entry fields are empty. See the  `User role/profile Page <#user-role-profile-page>`__. for information on the data entry and mandatory fields.

Editing a User role/profile
"""""""""""""""""""""""""""


  Click on the Edit button to re-direct to the  `User role/profile Page <#user-role-profile-page>`__.

  The page will open with the current information loaded into the data entry fields. See the `User role/profile Page <#user-role-profile-page>`__. for information on the data entry and mandatory fields.

Duplicating a User role/profile
"""""""""""""""""""""""""""""""

  Click on the Duplicate button to re-direct to the `User role/profile Page <#user-role-profile-page>`__.

  The page will open with all the current rights for the selected user role/profile, (except for theuser role/profile name which should be unique), loaded into the data entry fields. See the `User role/profile Page <#user-role-profile-page>`__ for information on the data entry and mandatory fields. To save the record, enter a unique code before clicking on ``Save``.


Deleting a User role/profile
""""""""""""""""""""""""""""

  Click on the Delete button to delete the currently selected record.

  Before deleting a confirmation popup (:ref:`Image User roles/profile delete confirmation <user_role_delete>`) is displayed, this requires the user to confirm if the action should really be carried out.

      .. _user_role_delete:
      .. figure:: /img/user_manual/user_role_delete.png
         :align: center

         `User roles/profile delete confirmation`

  When a user roles/profile is deleted, the rights that it provide are not available to the users having that role/profile.

Default User roles and rights
"""""""""""""""""""""""""""""

The table below shows the default roles in openIMIS.

  .. list-table:: Overview of Scheme administrator & district Staff roles
      :widths: 2 6 4
      :header-rows: 1
      :stub-columns: 1
      :class: longtable

      * - **Role**
        - **Responsibilities**
        - **Available functionality**

      * - Enrolment Officer
        - He/she enrols insurees and submits enrolment forms to a health insurance administration; handles policy modifications; collects feedback from scheme patients and submits to the health insurance administration.
        - | * Capture a photo of an Insuree.
          | * Send a photo
          | * Inquiry on an Insuree
          | * Collect feedback from an Insuree

      * - | Village Executive
          | Officer (VEO)
        - He/she collects feedbacks and collects changes on insurees during insurance periods
        - | * Collect feedback from an Insuree
          | * Inquiry on an Insuree

      * - Manager
        - Oversees operations of the health insurance scheme;runs openIMIS operational reports analyses data generated from the IMIS.
        - | * Create managerial statistics
          | * Authorize issuance of a substitution
          | * membership card

      * - Accountant
        - Transfers data on collected Contributions to an external accounting system. Calculates claim amounts per health facility, runs openIMIS operational reports and presents claims decision overview to management of a health insurance administrator. Processes approved claims to health facility sub-accounts.
        - | * Transfer of data on Contributions to accounting system
          | * Valuation of a claim
          | * Transfer of a batch of claims for payment

      * - Clerk
        - Enters and modifies data on families, insurees, policies and contributions. Enters data on claims if the claims are submitted in a paper form.
        - | * `Creation/ Search/ Modification/ Deletion/ Modification <#family-group-page>`__ of a `household/group <#family-overview-page>`__, an `Insuree <#insuree-page>`_, a `Policy <#policy-page>`__ or a `Contribution <#contribution-page>`__.
          | * `Renewal of a policy <#policy-renewals>`__
          | * `Entry of a claim <#claim-page>`__

      * - Medical Officer
        - Provides technical advice on claims verification from a medical standpoint.
        - | * Checking of a claim for plausibility
          | * `Review of a claim <#policy-renewals>`__
          | * `Authorize a claim for payment <#claim-page>`__

      * - | Scheme
          | Administrator
        - Administers registers (all except the register of users)
        - | * `Administer registers <#administration-of-registers>`__ ( `Officers, Payers, Health Facilities <#health-facilities-administration>`__, , `Medical Services, Medical Items, Medical Item Price Lists, Medical Services Price List <#medical-service-price-lists-administration>`__, `Products <#claim-administrators-administration>`__)
          | * `Extract Creation for Off-line Health Facilities <#imis-extracts-online-mode>`__

      * - | openIMIS
          | Administrator
        - Administers operations of the IMIS. Is responsible for backups of data.
        - | * Administer the register of `users <#user_administration>`__, `Utilities <#utilities>`__
          | * Manage `Backup <#backup>`__, `Restore <#restore>`__ and `Updates <#execute-script>`__
          | * `Extract Creation for Off-line Health Facilities <#imis-extracts-online-mode>`__

  .. list-table:: Overview of Health Facilities staff roles
      :widths: 2 6 4
      :header-rows: 1
      :stub-columns: 1

      * - **Role**
        - **Responsibilities**
        - **Available functionality**
      * - Receptionist
        - Verifies membership and issues to a patient a claim form.
        - | * Inquiring on a Household/group, `Insuree <#find-insuree>`__ and `Policy <#find-policy>`__

      * - | Claim
          | Administrator
        - Pools claim forms of a health facility, enters and submits claims.
        - | * Opening of a batch of claims
          | * Entry of a claim

      * - | HF
          | Administrator
        - Off-line HealthFacility administration
        - | * `Off-line extract upload <#imis-extracts-offline-mode>`__

      * - | Offline HF
          | Administrator
        - Off-line HealthFacility administration
        - | * Creation of clerk
          | * Creation of offline Extract
