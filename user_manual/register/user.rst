Users administration
^^^^^^^^^^^^^^^^^^^^

  User administration is restricted to users with the system role of IMIS Administrator or with a role including an access to Administration/Users.

Pre-conditions
""""""""""""""

  A user may only be added or thereafter edited, after the approval of the management of the scheme administration. Deletion of a user normally will occur when a user leaves his/her post within the health insurance scheme and/or the scheme administration. A built in user with the user name Admin and the initial password Admin is created automatically in IMIS with access to all locations of the register of locations (at any time). The Admin user has an implicit role that includes full access rights to the registers of locations, full access to the register of user profiles and an access to downloading/uploading of the register of locations to/from an external file.

Navigation
""""""""""

  All functionality for use with the administration of users can be found under the main menu ``Administration``, sub menu ``Users``.

  .. _image52:
  .. figure:: /img/user_manual/image45.png
    :align: center

    `Image 52 - Navigation Users`

  Clicking on the sub menu ``Users`` re-directs the current user to the `User Control Page <#user-control-page>`__\ .

  .. _image53:
  .. figure:: /img/user_manual/image46.png
    :align: center

    `Image 53 - User Control Page`

User Control Page
"""""""""""""""""

  The ``User Control Page`` is the central point for all user administration. By having access to this page, it is possible to add, edit, delete and search users. The page is divided into four panels (:ref:`Image 52<image52>`).

  The following rules apply to the list of found users besides conformance with all search criteria:

    #.  The user Admin is not included in any searching for users with exception of  searching done by an Admin user itself.

    #.  A user having access rights Users/Search (see User Profiles) can get as a result of a searching only users that have access to same set of locations or to a subset of locations of the searching user only.


 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. In the case of users the following search options are available which can be used alone or in combination with each other.

    * ``Last Name``

      Type in the beginning of; or the full Last name; to search for users with a Last name, which starts with or matches completely, the typed text.

    * ``Login Name``

      Type in the beginning of; or the full Login name, to search for users with a Login name, which starts with or matches completely, the typed text.

    * ``Phone Number``

      Type in the beginning of; or the full Phone Number, to search for users, with a Phone Number which starts with or matches completely, the typed text.

    * ``Email``

      Type in the beginning of; or the full Email, to search for users, with an Email which starts with or matches completely, the typed text.

    * ``Other Names``

      Type in the beginning of; or the full Other Names, to search for users, with Other names which start with or match completely the typed text.

    * ``Role``

      Select the Role; from the list of roles by clicking on the arrow on the right of the selector, to select users of a specific role.

    * ``Health Facilities``

      Select the Health Facility; from the list of health facilities by clicking on the arrow on the right of the selector, to select users from a specific health facility. *Note: The list will only be filled with the health facilities belonging to the districts assigned to the currently logged in user.*

    * ``Region``

      Select the Region; from the list of regions by clicking on the arrow on the right of the selector to find users with access to a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user.*

    * ``District``

      Select the District; from the list of districts by clicking on the arrow on the right of the selector to find users with access to a specific district. *The list will be only filled with the districts belonging to the selected region.*

    * ``Language``

      Select the Language; from the list of languages by clicking on the arrow on the right of the selector, to select users with a specific language.

    * ``Historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records (:ref:`Image 54<image54>`).

    .. _image54:
    .. figure:: /img/user_manual/image47.png
      :align: center

      `Image 54 - Historical records - Result Panel`

    * ``Search Button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the result panel.

 #. **Result Panel**

    .. _image55:
    .. figure:: /img/user_manual/image48.png
      :align: center

      `Image 55 - Selected record (blue), hovered records (yellow) - Result Panel`

    The result panel displays a list of all users found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 55<image55>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:ref:`Image 56<image56>`)

    .. _image56:
    .. figure:: /img/user_manual/image11.png
      :align: center

      `Image 56 - Page selector- Result Panel`

 #. **Button Panel**

    With exception of the ``Cancel`` button, which re-directs to the `Home Page <#image-2.2-home-page>`__, and the ``Add`` button which re-directs to the `User Page <#user-page>`__, the button panel (the buttons ``Edit`` and ``Delete``) is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a user has been added, updated or deleted or if there was an error at any time during the process of these actions.

­User Page
""""""""""

 #. **Data Entry**

    .. _image57:
    .. figure:: /img/user_manual/image49.png
      :align: center

      `Image 57 - User Page`

    * ``Language``

      Select the user’s preferred language from the list by clicking on the arrow on the right hand side of the lookup. Mandatory.

    * ``Last name``

      Enter the last name (surname) for the user. Mandatory, 100 characters maximum.

    * ``Other Names``

      Enter other names of the user. Mandatory, 100 characters maximum.

    * ``Phone Number``

      Enter the phone number for the user. 50 characters maximum.

    * ``Email``

      Enter the e-mail address for the user. 50 characters maximum.

    * ``Login Name``

      Enter the Login name for the user. This is an alias used for logging into the application; a minimum of 6 and a maximum of 25 characters should be used for the login. Each Login Name should be unique. Mandatory.

    * ``Password``

      Enter the password for the user. This is used at login to grant access to the application; a minimum of 8 and a maximum of 25 characters should be used for the password. The password should have at least one digit. Mandatory.

    * ``Confirm Password``

      Re-enter the password. The password must be entered twice, to ensure that there was no mistyping in the first entry. Mandatory.

    * ``Health Facility``

      Select the health facility that the user belongs to, if applicable, from the list of health Facilities from the list by clicking on the arrow on the right hand side of the lookup. *Note: The list will only be filled with the Health Facilities belonging to the districts assigned to the currently logged in user.*

    * ``Roles``

      Select from the list of available roles the Roles which the user carries out, by either clicking on the ``Check All`` box at the top of the list of Roles, or by selectively clicking on the ``Check box`` to the left of the role. Mandatory (at least one role must be selected). The list of roles contains all roles (user profiles) that are not blocked. Mandatory (at least one role must be selected)

    * ``Regions``

      Select from the list of available regions the region(s) which the user will have access to, by either clicking on the ``Check All`` box at the top of the list of regions, or by selectively clicking on the ``Check box`` to the left of a region. Mandatory (at least one region must be selected). The selection can be done indirectly by selecting a district or some districts. The box contains only regions accessible to the user or regions that have been added by the user. Mandatory (at least one region must be selected). The selection can be done indirectly by selecting a district or some districts.

    * ``Districts``

      Select from the list of available districts the district(s) which the user will have access to, by either clicking on the ``Check All`` box at the top of the list of districts, or by selectively clicking on the ``Check box`` to the left of the district. Districts are pre-selected based on the selected region(s). The pre-selection can be modified. Mandatory (at least one district must be selected). The selection can be done indirectly by just selecting a region or some regions. The box contains only regions accessible to the user or regions that have been added by the user. Mandatory (at least one region must be selected). The selection can be done indirectly by selecting a district or some districts.

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `User Control Page <#user-control-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the user has been saved will appear on the Information Panel.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data fields will take the focus (by an asterisk on the right of the corresponding data field).

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `User Control Page. <#user-control-page>`__

Adding a User
"""""""""""""

  Click on the Add button to re-direct to the `User Page <#user-page>`__.

  When the page opens all entry fields are empty. See the `User Page <#user-page>`__ for information on the data entry and mandatory fields.

Editing a User
""""""""""""""

  Click on the Edit button to re-direct to the `User Page <#user-page>`__

  The page will open with the current information loaded into the data entry fields. See the `User Page <#user-page>`__ for information on the data entry and mandatory fields

Deleting a User
"""""""""""""""

  Click on the Delete button to delete the currently selected record

  Before deleting a confirmation popup (:ref:`Image 58<image58>`) is displayed, this requires the user to confirm if the action should really be carried out.

  .. _image58:
  .. figure:: /img/user_manual/image24.png
    :align: center

    `Image 58 - Delete confirmation- Button Panel`

  When a user is deleted, all records retaining to the deleted user will still be available by selecting historical records.
