Users Administration
^^^^^^^^^^^^^^^^^^^^

User administration is restricted to users with the system role of IMIS Administrator or with a role including an access to Administration/Users.

Enrolment officers and Claim administrators are now considered as a user with specific roles.

.. contents:: Table of Contents


Pre-conditions
==============

A user may only be added or edited after the approval of the management of the scheme administration. Deletion of a user normally will occur when a user leaves his/her post within the health insurance scheme and/or the scheme administration. A built in user with the user name Admin and the initial password Admin is created automatically in openIMIS with access to all locations of the register of locations (at any time). The Admin user has an implicit role that includes full access rights to the registers of locations, full access to the register of user profiles and an access to downloading/uploading of the register of locations to/from an external file.

Navigation
==========

All functionalities related to users administration can be found under the main menu ``Administration``, sub menu ``Users``.

.. figure:: /img/user_manual/users_navigation.png
  :align: center

  `Navigation to users page`

Clicking on the sub menu ``Users`` redirects the current user to the `Users List Page <#users-list-page>`__\ .

.. figure:: /img/user_manual/users_list.png
  :align: center

  `User List Page`

Users List Page
================

It is the central point for the users administration. By having access to this page, it is possible to add, edit, delete and search users. The page is divided into four panels.

The following rules apply to the list of found users besides conformance with all search criteria:

  #. The user Admin is not included in any search for users with exception of searches done by an Admin user itself.

  #. A user having the access right *Users/Search* (see :ref:`User Profiles <user_roles_control_page>`) will only be able to see users that have access to them same set of locations or to a subset of locations of the user making the search only.


Search Panel
""""""""""""

The search panel allows a user to filter on specific criteria.

Last Name
  Filter on users who have the typed text in their last name. 

Login Name
  Filter on users who have the typed text in their login. 

Phone Number
  Filter on users who have the typed text in their phone number. 

Email
  Filter on users who have the typed text in their email. 

Other Names
  Filter on users who have the typed text in their other names. 

Role
  Filter users with the selected role

Health Facilities
  Select the Health Facility; from the list of health facilities by clicking on the arrow on the right of the selector, to select users from a specific health facility. 
  
  .. note::
    The list will only contain the health facilities belonging to the districts assigned to the currently logged in user.

Region
  Select the Region from the list of regions by clicking on the arrow on the right of the selector to find users with access to a specific region.
  
  .. note::
    The list will only contain the health facilities belonging to the regions assigned to the currently logged in user.


District
  Select the District from the list of districts by clicking on the arrow on the right of the selector to find users with access to a specific district.

  .. note::
    The list will only contain the health facilities belonging to the districts assigned to the currently logged in user.

Language
  Select the Language from the list of languages by clicking on the arrow on the right of the selector, to select users with a specific language.

Search Button
  Once the criteria have been entered, use the search button to filter the records, the results will appear in the result panel.

Results Panel
"""""""""""""""

.. _users_results:
.. figure:: /img/user_manual/users_results.png
  :align: center

  `Selected record (blue), hovered records (yellow) - Results Panel`

The result panel displays a list of all users found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:numref:`users_results`). The leftmost record contains a hyperlink which if clicked, redirects the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:numref:`users_pagination`)

.. _users_pagination:
.. figure:: /img/user_manual/users_pagination.png
  :align: center

  `Page selector- Results Panel`

Buttons Panel
""""""""""""""

With exception of the ``Cancel`` button, which redirects to the :ref:`Home Page <home_page>`, the button panel (the buttons ``Edit`` and ``Delete``) is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

Information Panel
""""""""""""""""""

The Information Panel is used to display messages back to the user. Messages will occur once a user has been added, updated or deleted or if there was an error at any time during the process of these actions.

­User Page
==========

.. _users_form:
.. figure:: /img/user_manual/users_form.png
  :align: center

  `User Page`

Fields
""""""""

Generic Fields
--------------

User name
  Enter the Login name for the user. This is an alias used for logging into the application; a minimum of 6 and a maximum of 25 characters should be used for the login. Each Login Name should be unique. Mandatory.

Given Names
  Enter other names of the user. Mandatory, 100 characters maximum.

Last name
  Enter the last name (surname) for the user. Mandatory, 100 characters maximum.

Email
  Enter the e-mail address for the user. 50 characters maximum.

Phone Number
  Enter the phone number for the user. 50 characters maximum.

Health Facility
  Select the health facility that the user belongs to, if applicable, from the list of health Facilities from the list by clicking on the arrow on the right hand side of the lookup.
  
  .. :note::
    The list will only be filled with the Health Facilities belonging to the districts assigned to the currently logged in user.

Roles
  Select from the list of available roles the Roles which the user carries out. Mandatory (at least one role must be selected). The list of roles contains all roles (user profiles) that are not blocked.

Districts
  Select from the list of available districts the district(s) which the user will have access to. Mandatory (at least one district must be selected). 
  
  .. :note::
    The box contains only regions accessible to the user or regions that have been added by the user.

Login Fields
--------------

Language
  Select the user’s preferred language from the list by clicking on the arrow on the right hand side of the lookup. Mandatory.

Password
  Enter the password for the user. This is used at login to grant access to the application; a minimum of 8 and a maximum of 25 characters should be used for the password. The password should have at least one digit. Mandatory.

Confirm Password
  Re-enter the password. The password must be entered twice, to ensure that there was no mistyping in the first entry. Mandatory.

Enrolment Officer Fields
------------------------

Birth date
  Birth date of the enrolment officer.

Works to
  End date at which the enrolment officer is replaced by the substitution officer.

Substitution Officer
  Replacement of the user after the `Works to` date.

Address
  Address of the living place of the enrolment officer.

Region & District
  Select the region & district where the enrolment officer will work. It will be used to select villages managed by the enrolment officer.

Villages
  List of all villages where enrolment officer will work. To add villages, you first need to add a row and select the municipality.

  .. figure:: /img/user_manual/users_enrolment_officer_villages.png
    :align: center

    `Enrolment Officer - Manage villages`

Claim Administrator Fields
---------------------------

Birth date
  Birth date of the enrolment officer.



Saving
""""""

Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be redirected back to the `User List Page <#user-list-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the user has been saved will appear on the Information Panel.

**Mandatory fields**

  If mandatory fields are not filled when the user clicks on the ``Save`` button, a message will appear in the Information Panel, and the data fields will take the focus (by an asterisk on the right of the corresponding data field).

**Cancel**

  By clicking on the ``Cancel`` button, the user will be redirected to the `Users List Page. <#user-list-page>`__

Adding a User
"""""""""""""

Click on the Add button to redirect to the `User Page <#user-page>`__.

When the page opens all entry fields are empty. See the `User Page <#user-page>`__ for information on the data entry and mandatory fields.

Editing a User
""""""""""""""

Click on the Edit button to redirect to the `User Page <#user-page>`__

The page will open with the current information loaded into the data entry fields. See the `User Page <#user-page>`__ for information on the data entry and mandatory fields

Deleting a User
"""""""""""""""

Click on the Delete button to delete the currently selected record

Before deleting a confirmation popup is displayed, this requires the user to confirm if the action should really be carried out.
