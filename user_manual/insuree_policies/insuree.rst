

Insuree
^^^^^^^

.. contents:: Table of Contents

Find Insuree
============

Access to the Find Insuree Page is restricted to users with the system roles of Accountant, Clerk and Health Facility Receptionist or with a role including an access to Insurees and Families/Insuree/Search.

Pre-conditions
--------------

Need to enquire on, or edit an insuree, and the family/group, policies and contributions associated.

Navigation
-----------

All functionality for use with the administration of insurees can be found under the main menu ``Insurees and Policies``, sub menu ``Insurees``.

.. _image75_insuree:
.. figure:: /img/user_manual/image75.png
  :align: center

  `Navigation Insurees`

Clicking on the sub menu ``Insurees`` re-directs the current user to the Find Insuree Page.

Page
----

.. _image96_insuree_search:
.. figure:: /img/user_manual/76_insuree_search.png
  :align: center

  `Find Insuree Page`

The ``Find Insuree Page`` is the first step in the process of finding an insuree and thereafter accessing the family/group overview of insurees, policies and contributions. This initial page can be used to search for specific Insurees or groups of insurees based on specific criteria. The panel is divided into three panels (:numref:`image96_insuree_search`)

A. Search Panel
""""""""""""""""

The Search Panel allows a user to select specific criteria to reduce the search results. In the case of insurees the following search options are available, which can be used alone or in combination with each other.

Region
  Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select insurees from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected.*

District
  Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to select insurees from a specific district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected.*

Municipality
  Select the ``Municipality``; from the list of wards either by typing at least two characters or by clicking on the arrow on the right of the selector to select insurees from a specific municipality. *Note: The list will only be filled with the wards in the selected district above.*

Village
  Select the ``Village``; from the list of villages either by typing at least two characters or by clicking on the arrow on the right of the selector to select insurees from a specific village. *Note: The list will only be filled with the villages in the selected municipality above.*

Insurance Number
  Type in the beginning of; or the full ``Insurance Number`` to search for insurees with the ``Insurance Number``, which starts with or matches completely, the typed text.

Last Name
  Type in the beginning of; or the full ``Last name``; to search for insurees with a ``Last name``, which starts with or matches completely, the typed text.

Given Names
  Type in the beginning of; or the full ``Given Names`` to search for insurees with ``Other Names`` which starts with or matches completely, the typed text.

Gender
  Select the ``Gender``; from the list of genders by clicking on the arrow on the right of the selector, to select insurees of a specific gender.

Marital Status
  Select the ``Marital Status``; from the list of marital status by clicking on the arrow on the right of the selector, to select insurees of a specific marital status.

Email
  Type in the beginning of; or the full ``Email`` address to search for insurees with a ``Email``, which contains or matches completely, the typed email.

Phone Number
  Type in the beginning of; or the full ``Phone Number`` to search for insurees with a ``Phone Number``, which contains or matches completely, the typed number.

Birth Date From
  Type in a date; or use the Date Selector Button, to enter the ``Birth Date From`` to search for insurees who have the same or later birth date. *Note. To clear the date entry box; click on the date and use the ``Clear`` button on the bottom left.*

Birth Date To
  Type in a date; or use the Date Selector Button, to enter the ``Birth Date To`` to search for insurees who have the same or earlier birth date. *Note. To clear the date entry box; click on the date and use the ``Clear`` button on the bottom left.*

Photo status
  Select whether all insurees are searched [**Any**] or only insurees [**With**] a photo assigned or only insurees [**Without**] photo assigned.

Show historical values
  Click on Show historical values to see historical records matching the selected criteria. Historical records are displayed in the result as grayed out. (:numref:`image98`)

  .. _image98:
  .. figure:: /img/user_manual/77_insuree_historical.png
    :align: center

    `Historical records - Result Panel`

Search Buttons
  When criteria are defined and potentially after a small delay, the search will be automatically executed. There are however two buttons on the top right:

  .. _image_search_buttons:
  .. |search_reset_button| image:: /img/user_manual/search_reset_button.png
    :align: middle
  .. |search_button| image:: /img/user_manual/search_button.png
    :align: middle

  +-----------------------+-----------------------+
  | |search_reset_button| | Reset search criteria |
  +-----------------------+-----------------------+
  | |search_button|       | Search (again)        |
  +-----------------------+-----------------------+

B. Result Panel
""""""""""""""""

The result panel displays a list of all Insurees found, matching the selected criteria in the search panel. The leftmost column contains a search icon which if clicked, opens a dialog with further details and eligibility check. On the right, the family icon directs the user to the `Family Overview Page <#family-overview-page.>`__ of the insuree’s family, and a button to delete the insuree.

.. _image_78_insuree_search_results:
.. figure:: /img/user_manual/78_insuree_search_results.png
  :align: center

  `Highlighted result row`

The number of rows per page is limited to 10 by default but one can use the "Rows per page" drop-down in the bottom right of the search results. If there are more rows to display, one can use the page navigation. (:numref:`image_100_insuree_edit`)

.. _image_79_pagination:
.. figure:: /img/user_manual/79_pagination.png
  :align: center
  :width: 50%

  `Page selector- Result Panel`

C. Information/Button Panel
"""""""""""""""""""""""""""

The Information Panel is used to display messages back to the user. Messages will occur once a insuree has been added, updated or deleted or if there was an error at any time during the process of these actions.

The ``+`` button will create a new insuree.


Insuree Page
============

  .. _image_100_insuree_edit:
  .. figure:: /img/user_manual/100_insuree_edit.png
    :align: center

    `Insuree Page`

#. **Family Details**

    The first section contains the family information. Refer to the Family section for details about the displayed fields.

#. **Insuree Data**

    Relationship
      Shown in the insuree section header only if the insuree is not the head of the family. Select from the list of available relationships of the insuree to the head of family/group.

    Insurance Number
      Enter the insurance number for the insuree. Mandatory.

    Last name
      Enter the last name (surname) for the insuree. Mandatory, 100 characters maximum.

    Given Names
      Enter given names of the insuree. Mandatory, 100 characters maximum.

    Birth Date
      Enter the date of birth for the insuree.

    Gender
      Select from the list of available genders the gender of the insuree. Mandatory.

    Marital Status
      Select from the list of available options for the marital status of the insuree.

    Beneficiary Card
      Select from the list of options whether or not the card was issued to the insuree.

    Photo Date
      Select the date at which the picture was taken.

    Photo
      Click on the person icon to upload a photo for the insuree related to his/her insurance number.

      *Note: There is an automated service in the openIMIS Server which will run on configured time basis repeatedly and assign related photos to insurees without photos if any exist in the openIMIS database. So after a user has input insuree's insurance number and no photo is displayed, there is no need to browse for the photo as that process will be done automatically by the service if the service is configured.*

    Officer
      Select the officer handling the insuree. Mandatory.

    Same Village as Family
      If selected, the village of the family is used for this insuree too. Otherwise, fields will appear with Region, District, Ward and Village selection.

    Same Address as Family
      If selected, the address of the family is used for this insuree too. Otherwise, an address field will appear to provide the actual address.

    Phone Number
      Enter the phone number for the insuree.

    Email
      Enter the e-mail address of the insuree.

    Profession
      Select from the list of available professions the profession of the insuree.

    Education
      Select from the list of available educations the education of the insuree.

    Identification Type
      Select the type of the identification document of the insuree.

    Identification No.
      Enter alphanumeric identification of the document of the insuree.

    First Service Point
      Region of FSP
        Select from the list of available regions the region, in which the chosen primary health facility (First Service Point) of the insuree is located.

      District of FSP
        Select from the list of available districts the district, in which the chosen primary health facility (First Service Point) of the insuree is located. *Note: The list will only be filled with the districts belonging to the selected region.*

      Level of FSP
        Select the level of the chosen primary health facility (First Service Point) of the insuree.

      First Service Point
        Select from the list of available health facilities the chosen primary health facility (First Service Point) of the insuree. *Note: The list will only be filled with the health facilities belonging to the selected district which are of the selected level.*


#. **Saving**

    .. image:: /img/user_manual/save_button.png
       :width: 69px
       :align: right

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Family Overview Page <#family-overview-page.>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the insuree has been saved will appear on the Information Panel.

    **Mandatory data**

    The ``Save`` button is disabled until all mandatory data fields (with an asterisk) are filled.
  
    **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Family Overview Page <#family-overview-page.>`__.

Adding an Insuree
=================

  Click on the Green Plus Sign to re-direct to the `Insuree Page <#insuree-page>`__\.

  When the page opens all entry fields are empty. See the `Insuree Page <#insuree-page>`__ for information on the data entry and mandatory fields.

Editing an Insuree
==================

  Double-click in the insuree search results to edit in the `Insuree Page <#insuree-page>`__\.

  The page will open with the current information loaded into the data entry fields. See the Insuree Page for information on the data entry and mandatory fields.

Deleting an Insuree
===================

  Click on trashcan icon on the right of an insuree search result to delete it.

  .. _image127a:
  .. figure:: /img/user_manual/delete_insuree_button.png
     :align: center
     :width: 250px

     `Delete insuree button`

  Before deleting a confirmation popup (:numref:`image127b`) is displayed, which requires the user to confirm if the action should really be carried out?

  .. _image127b:
  .. figure:: /img/user_manual/24_insuree_delete_confirmation.png
    :align: center

    `Insuree Delete confirmation`

  When an insuree is deleted, all records retaining to the deleted insuree will still be available by selecting historical records.
