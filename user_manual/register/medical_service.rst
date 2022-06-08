

Medical Services
^^^^^^^^^^^^^^^^

  The register of Medical Services contains all medical services that can be included in packages of benefits of insurance products administered and remunerated by the health insurance scheme. Administration of the register of medical services is restricted to users with the system role of Scheme Administrator or with a role including an access to Administration/Medical Services.

Pre-conditions
""""""""""""""

  A medical service may only be added or thereafter edited or deleted, after the approval of the management of the scheme administration.

Navigation
""""""""""

  All functionality for use with the administration of Medical Services can be found under the main menu ``Administration``, sub menu ``Medical Services.``

  .. _medical_service.menu:
  .. figure:: /img/user_manual/medical_service.menu.png
    :align: center

    `Navigation Medical Services`

  Clicking on the sub menu ``Medical Services`` re-directs the current user to the `Medical Services Control Page <#medical-services-control-page>`__\.

  .. _medical_service.search:
  .. figure:: /img/user_manual/medical_service.search.png
    :align: center

    `Medical Services Control Page`

Medical Services Control Page
"""""""""""""""""""""""""""""

  The ``Medical Services Control Page`` is the central point for all medical service administration. By having Access to this panel, it is possible to add, edit, delete and search. The panel is divided into four panels (:numref:`medical_service.search`)

 #. **Search Panel**

    The Search Panel allows a user to select specific criteria to minimise the search results. In the case of medical services the following search options are available which can be used alone or in combination with each other.

    Code
      Type in the beginning of; or the full ``Code``; to search for medical services with a ``Code``, which starts with or matches completely, the typed text.

    Name
      Type in the beginning of; or the full ``Name`` to search for medical services with a ``Name``, which starts with or matches completely, the typed text.

    Type
      Select the ``Type``; from the list of types (Preventive, Curative) by clicking on the arrow on the right of the selector, to select medical services of a specific type.

    * ``Historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in grey and with a Valid date to clearly define them from current records (:numref:`medical_service.history`)

      .. _medical_service.history:
      .. figure:: /img/user_manual/medical_service.history.png
        :align: center

        `Historical records - Result Panel`

    Search Button
      Once the criteria have been entered, use the search button to filter the records, the results will appear in the result panel.

 #. **Result Panel**

    The Result Panel displays a list of all medical services found, matching the selected Criteria in the search panel. Double click re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.


   A maximum of 10 records are displayed at one time( can be changed :numref:`mat_page_browser`), further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:numref:`mat_record_per_page`)


 #. **Button Panel**

    * Material UI  add button can be used to add medical items

    * Double click on a line open the service

    * Delete button at the end of the line delete the service

    * "Open in new tab" button enable the user to open the service in a new tab.


 #. **Information Panel**

      `Page selector- Result Panel`

Medical Service Page
""""""""""""""""""""

 #. **Data Entry**

    .. _medical_service.edit:
    .. figure:: /img/user_manual/medical_service.edit.png
      :align: center

      `Medical Service Page`

    Code
      Enter the code for the medical service. Mandatory, 6 characters.

    Name
      Enter the name of the medical service. Mandatory, 100 characters maximum.

    Category
      Choose the category (Surgery, Consultation, Delivery, Antenatal, Other) which the medical service belongs to.

    Type
      Choose one from the options available (Preventive, Curative), the type of the medical service. Mandatory.

    * ``Service Level``

      Select from the list (Simple Service, Visit, Day of Stay, Hospital Case), the level for the medical service. Mandatory.

    Price
      Enter the price a general price that can be overloaded in pricelists. Full general price (including potential cost sharing of an insuree) for the medical service. Mandatory.

    Care Type
      Choose one from the options available (Out-patient, In-patient, Both), the limitation of provision of the medical service to the specific type of health care. Mandatory.

    Frequency
      Enter the limitation of frequency of provision in a number of days within which a medical service can be provided to a patient not more than once. If the frequency is zero, there is no limitation. *Note: By default the frequency is 0.*

    Patient
      Choose one or a combination of the options available, to specify which patient type the medical service is applicable to. *Note: By default all patient options are checked (selected).*

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Medical Services Control Page <#medical-services-control-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the medical service has been saved will appear on the Information Panel.

 #. **Mandatory data**

    If mandatory data is not entered the ``Save`` button won't be active


Adding a Medical Service
""""""""""""""""""""""""

  Click on the ``Add`` button to re-direct to the `Medical Service Page <#medical-service-page>`__\ .

  When the page opens all entry fields are empty. See the `Medical Service Page <#medical-service-page>`__ for information on the data entry and mandatory fields.

Editing a Medical Service
"""""""""""""""""""""""""

  Double click on the service line to re-direct to the `Medical Service Page <\l>`__\ .

  The page will open with the current information loaded into the data entry fields. See the `Medical Service Page <#medical-service-page>`__ for information on the data entry and mandatory fields.

Deleting a Medical Service
""""""""""""""""""""""""""

  Click on the ``<`` button to delete the currently selected record; the user is re-directed the `Medical Services Control Page <#medical-services-control-page>`__\.

  Before deleting a confirmation popup (:numref:`image28`) is displayed, which requires the user to confirm if the action should really be carried out?

  .. _image28:
  .. figure:: /img/user_manual/med_service_delete.png
    :align: center
    :width: 50%

    `Delete confirmation- Button Panel`

  When a medical service is deleted, all records retaining to the deleted medical service will still be available by selecting historical records.
