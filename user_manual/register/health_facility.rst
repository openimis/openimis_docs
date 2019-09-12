.. include:: /_sidebar.rst.inc

Health Facilities Administration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  The register of health facilities contains all health facilities contracted and/or eligible for submitting of claims by/to the health insurance scheme. Health Facility administration is restricted to users with the system role of Scheme Administrator or with a role including an access to Administration/Health Facilities.

Pre-conditions
""""""""""""""

  A health facility may only be added if the management of the scheme administration contracts it or if eligibility of submitting of claims can be derived from the legislation. It may thereafter be edited; however, approval of the management of the scheme administration is required for a change of the pricelists associated with the health facility. Deletion of a health facility normally will occur when a Health Facility stops its activity or the contract with the health facility with the scheme administration is cancelled.

Navigation
""""""""""

  .. _image15:
  .. figure:: /img/user_manual/image19.png
    :align: center

    `Image 15 - Navigation Health Facilities`

  All functionality for use with the administration of health facilities can be found under the main menu ``Administration``, sub menu ``Health Facilities.``

  Clicking on the sub menu ``Health Facilities`` re-directs the current user to the `Health Facilities Control Page <#health-facilities-control-page>`__\.

  .. _image16:
  .. figure:: /img/user_manual/image20.png
    :align: center

    `Image 16 - Health Facilities Control Page`

Health Facilities Control PAGE
""""""""""""""""""""""""""""""

  The ``Health Facilities Control Page`` is the central point for all health facilities administration. By having access to this page, it is possible to add, edit, delete and search. The page is divided into four panels (:ref:`Image 16<image16>`)

 #. **Search Panel**

    The Search Panel allows a user to select specific criteria to minimise the search results. In the case of health facilities the following search options are available which can be used alone or in combination with each other.

    * ``Code``

      Type in the beginning of; or the full ``Code``; to search for health facilities with a ``Code``, which starts with or matches completely, the typed text.

    * ``Name``

      Type in the beginning of; or the full ``Name``; to search for health facilities with a ``Name``, which starts with or matches completely, the typed text.

    * ``Fax``

      Type in the beginning of; or the full ``Fax`` to search for health facilities with a ``Fax``, which starts with or matches completely, the typed number.

    * ``Level``

      Select the ``Level``; from the list of levels of health facilities (Dispensary, Health Centre, Hospital) by clicking on the arrow on the right of the selector, to select health facilities of a specific level of service.

    * ``Phone Number``

      Type in the beginning of; or the full ``Phone Number`` to search for health facilities with a ``Phone Number``, which starts with or matches completely, the typed number.

    * ``Email``

      Type in the beginning of; or the full ``Email`` to search for health facilities with an ``Email`` which starts with or matches completely, the typed text.

    * ``Legal Form``

      Select the ``Legal Form``; from the list of legal forms (Government, District organization, Private Organisation, Charity) by clicking on the arrow on the right of the selector, to select health facilities of a specific legal form.

    * ``Region``

      Select the ``Region``; from the list of districts by clicking on the arrow on the right of the selector to select health facilities from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then this region will be automatically selected.*

    * ``District``

      Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to select health facilities from a specific district. *Note: The list will only be filled with the districts that belong to the selected region and that are assigned to the current logged in user. If this is only one then the district will be automatically selected.*

    * ``Care Type``

      Select the ``Care Type`` from the list of types (In-patient, Out-patient, Both) of provided health care by clicking on the arrow on the right of the selector, to select health facilities with a specific type.

    * ``Historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records (:ref:`Image 17<image17>`)

      .. _image17:
      .. figure:: /img/user_manual/image21.png
        :align: center

        `Image 17 - Historical Records - Result Panel`

    * ``Search button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the Result Panel.

 #. **Result Panel**

    The result panel displays a list of all health facilities found, matching the selected Criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 18<image18>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

      .. _image18:
      .. figure:: /img/user_manual/image22.png
        :align: center

        `Image 18 - Selected record (blue), hovered records (yellow) - Result Panel`

    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:ref:`Image 19<image19>`)

      .. _image19:
      .. figure:: /img/user_manual/image11.png
        :align: center

        `Image 19 - Page selector- Result Panel`

 #. **Button Panel**

    With exception of the ``Cancel`` button, which re-directs to the `Home Page <#image-2.2-home-page>`__, and the ``Add`` button which re-directs to the health facility page, the button panel (the buttons ``Edit`` and ``Delete)`` is used in conjunction with the current selected record (highlighted with blue). The user should select first a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a health facility has been added, updated or deleted or if there was an error at any time during the process of these actions.

Health Facility Page
""""""""""""""""""""

 #. **Data Entry**

    .. _image20:
    .. figure:: /img/user_manual/image23.png
      :align: center

      `Image 20 - Health Facility Page`

    * ``Code``

      Enter the code for the health facility. Mandatory, 8 characters.

    * ``name``

      Enter the name for the health facility. Mandatory, 100 characters maximum.

    * ``Legal Form``

      Select the legal form of the health facility from the list (Government, District organization, Private Organisation, Charity), by clicking on the arrow on the right hand side of the lookup.  Mandatory.

    * ``Level``

      Select a level from the list levels (Dispensary, Health Centre, Hospital), by clicking on the arrow on the right hand side of the lookup. Mandatory.

    * ``Sub Level``

      Select a sub-level from the list sub-levels (No Sublevel, Integrated, Reference), by clicking on the arrow on the right hand side of the lookup. Mandatory.

    * ``Address``

      Enter the address of the health facility. Mandatory, 100 characters maximum.

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow  on the right of the selector to enter the region in which the health facility is located. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then this region will be automatically selected.* Mandatory.

    * ``District``

      Select the ``district``; from the list of districts by clicking on the arrow on the right of the selector to enter the district in which the health facility is located. *Note: The list will only be filled with the districts assigned to the selected region and to districts assigned to the currently logged in user. If this is only one then the district will be automatically selected.* Mandatory.

    * ``Phone Number``

      Enter the phone number for the health facility. 50 characters maximum.

    * ``Fax``

      Enter the fax number for the health facility. 50 characters maximum.

    * ``Email``

      Enter the email for the health facility. 50 characters maximum.

    * ``Care Type``

      Select the type of health care provided by the health facility from the list (In-patient, Out-patient, Both), by clicking on the arrow on the right hand side of the lookup. Mandatory.

    * ``Price Lists (Medical Services)``

      Select the health facilities price lists (for medical services) from the list by clicking on the arrow on the right hand side of the lookup. The pricelist contains the list of medical services and their prices agreed between the health facility (or corresponding group of health facilities) and the scheme administration which can be invoiced by the health facility and remunerated by the scheme administration. *Note: The list will only be filled with the pricelists associated with the previously selected district, regional and nationwide pricelists assigned to the current logged in user.*

    * ``Price Lists (Medical Items)``

      Select the health facilities price lists (medical items) from the list by clicking on the arrow on the right hand side of the lookup. The pricelist contains the list of medical items and their prices agreed between the health facility (or corresponding group of health facilities) and the scheme administration which can be invoiced by the health facility and remunerated by the scheme administration. *Note: The list will only be filled with the pricelists associated with the previously selected district, regional and nationwide pricelists assigned to the current logged in user.*

    * ``Account Code``

      Enter the account code (Identification for the accounting software), which will be used in reports on remuneration to be received by the health facility. 25 characters maximum.

    * ``Region, District, Municipality, Village, Catchment grid``

      Check the locations that define the catchment area of the health facility. Specify the percentage of the population of a village that belong to the catchment area in the catchment column. Default is 100%.

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the ``Health Facility Control Page``, with the newly saved record displayed and selected in the result panel. A message confirming that the health facility has been saved will appear on the Information Panel.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right of the corresponding data field).

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Health Facilities Control Page <#health-facilities-control-page>`__.

Adding a Health Facility
""""""""""""""""""""""""

  Click on the ``Add`` button to re-direct to the `Health Facility Page <#health-facility-page>`__

  When the page opens all entry fields are empty. See the `Health Facility Page <#health-facility-page>`__ for information on the data entry and mandatory fields.

Editing a Health Facility
"""""""""""""""""""""""""

  Click on the ``Edit`` button to re-direct to the `Health Facility Page <#health-facility-page>`__\ .

  The page will open with the current information loaded into the data entry fields. See the `Health Facility Page <#health-facility-page>`__ for information on the data entry and mandatory fields

Deleting a Health Facility
""""""""""""""""""""""""""

  Click on the ``Delete`` button to delete the currently selected record.

  Before deleting a confirmation popup (:ref:`Image 21<image21>`) is displayed, which requires the user to confirm if the action should really be carried out?

    .. _image21:
    .. figure:: /img/user_manual/image24.png
      :align: center

      `Image 21 - Delete confirmation- Button Panel`

  When a health facility is deleted, all records retaining to the deleted health facility will still be available by selecting historical records.
