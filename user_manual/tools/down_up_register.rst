

Upload / Download selected registers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  Access to uploading/downloading of selected registers is restricted to the users with the the system role of IMIS Administrator ( the register of locations) or with a role including an access to Tools/Registers.

Navigation
""""""""""

  All functionality for use with the administration of uploading/downloading of selected registers can be found under the main menu ``Tools``, sub menu ``Registers``.

  .. _image166:
  .. figure:: /img/user_manual/tool.menu_register.png
    :align: center

    `Navigation to Registers`

  Clicking on the sub menu ``Registers`` re-directs the current user to the `Registers Page`: (:numref:`image166`)

Registers page
""""""""""""""

  .. _image167:
  .. figure:: /img/user_manual/image137.jpeg
    :align: center

    `Upload Registers`

  The Registers Page is divided into eight sections: (:numref:`image167`)

  A. Upload of the list of diagnoses

    * ``Browse``

      Select from a file in the XML format serving as a source for uploading of the list of diagnoses. Mandatory.

    * ``Strategy``

      Select a desired strategy for uploading of the list of diagnoses. The following options are available:

    * ``Insert Only``

      Uploads only diagnoses that are not yet included in the list of diagnoses

    * ``Update Only``

     Updates only diagnoses that are already included in the list of diagnoses

    * ``Insert and Update``

     Uploads diagnoses that are not yet included in the list of diagnoses and updates diagnoses that are already included in the list of diagnoses

    * ``Insert, Update and Delete``

     Uploads diagnoses that are not yet included in the list of diagnoses, updates diagnoses that are already included in the list of diagnoses and deletes diagnose that are not included in the source file

    * ``Dry Run``

      If checked, only diagnostics is provided without real uploading.

    * ``Upload``

      By clicking on the ``Upload`` button, a prompt popup message will appear, require a user to agree or disagree:(:ref:`image_upload_diagnoses`
       If user agrees the selected file containing diagnoses will be uploaded.

        .. _image_upload_diagnoses:
        .. figure:: /img/user_manual/image138.png
          :align: center

          `Upload Diagnoses`

      A statistics on the number of inserted/updated diagnoses appears:
        (:ref:`image_upload_diagnoses_statistics`).

        .. _image_upload_diagnoses_statistics:
        .. figure:: /img/user_manual/image139.png
          :align: center

          `Statistics on uploaded diagnoses`

     If there are errors an error protocol appears: (:ref:`image_upload_diagnoses_error`)

        .. _image_upload_diagnoses_error:
        .. figure:: /img/user_manual/image_upload_diagnoses_error.png
          :align: center

          `Error protocol on uploaded diagnoses`

    +--------------------------------------------------------------------------+
    | *DTD definition of the XML file for uploading/downloading of diagnoses:* |
    |                                                                          |
    |    <!DOCTYPE Diagnoses> [                                                |
    |                                                                          |
    |    <!ELEMENT Diagnoses (Diagnosis)*>                                     |
    |                                                                          |
    |    <!ELEMENT Diagnosis (DiagnosisCode, DiagnosisName)>                   |
    |                                                                          |
    |    < !ELEMENT DiagnosisCode (#CDATA)>                                    |
    |                                                                          |
    |    < !ELEMENT DiagnosisName (#CDATA)>                                    |
    |                                                                          |
    |    ]>                                                                    |
    +--------------------------------------------------------------------------+

  B. Upload of the register of locations

    * ``Browse``

      Select from a file in the XML format serving as a source for uploading of the register of locations. Mandatory.

    * ``Strategy``

      Select a desired strategy for uploading of the register of locations. The following options are available:

    * ``Insert Only``

      Uploads only locations that are not yet included in the register of locations

    * ``Update Only``

      Updates only locations that are already included in the register of locations

    * ``Insert and Update``

      Uploads locations that are not yet included in the register of locations and updates locations that are already included in the register of locations

    * ``Dry Run``

      If checked only diagnostics is provided without real uploading.

    * ``Upload``

      By clicking on the Upload button, a prompt popup message will appear, require a user to agree or disagree (:ref:`image_upload_locations`). If user agrees the selected file containing locations will be uploaded.

      .. _image_upload_locations:
      .. figure:: /img/user_manual/image_upload_locations.png
        :align: center

        `Upload Locations`

      A statistics on the number of inserted/updated locations appears
      (:ref:`image_upload_locations_statistics`)

      .. _image_upload_locations_statistics:
      .. figure:: /img/user_manual/image_upload_locations_statistics.png
        :align: center

        `Upload Locations statistics`

      If there are errors an error protocol appears (:ref:`image_upload_locations_error`)

      .. _image_upload_locations_error:
      .. figure:: /img/user_manual/image_upload_locations_error.png
        :align: center

        `Upload Locations error`

      +-----------------------------------------------------------------------+
      | *DTD definition of the XML file for uploading/downloading of          |
      | locations:*                                                           |
      |                                                                       |
      |    <!DOCTYPE Locations> [                                             |
      |                                                                       |
      |    <!ELEMENT Locations (Regions, Districts, Municipalities,           |
      |    Villages)>                                                         |
      |                                                                       |
      |    <!ELEMENT Regions (Region*)>                                       |
      |                                                                       |
      |    <!ELEMENT Region (RegionCode, RegionName)>                         |
      |                                                                       |
      |    < !ELEMENT RegionCode (#CDATA)>                                    |
      |                                                                       |
      |    < !ELEMENT RegionName (#CDATA)>                                    |
      |                                                                       |
      |    <!ELEMENT Districts (District*)>                                   |
      |                                                                       |
      |    <!ELEMENT District (RegionCode,DistrictCode, DistrictName)>        |
      |                                                                       |
      |    < !ELEMENT RegionCode (#CDATA)>                                    |
      |                                                                       |
      |    < !ELEMENT DistrictCode (#CDATA)>                                  |
      |                                                                       |
      |    < !ELEMENT DistrictName (#CDATA)>                                  |
      |                                                                       |
      |    <!ELEMENT Municipalities (Municipality*)>                          |
      |                                                                       |
      |    <!ELEMENT Municipality (DistrictCode,MunicipalityCode,             |
      |    MunicipalityName)>                                                 |
      |                                                                       |
      |    < !ELEMENT DistrictCode (#CDATA)>                                  |
      |                                                                       |
      |    < !ELEMENT MunicipalityCode (#CDATA)>                              |
      |                                                                       |
      |    < !ELEMENT MunicipalityName (#CDATA)>                              |
      |                                                                       |
      |    <!ELEMENT Villages (Village*)>                                     |
      |                                                                       |
      |    <!ELEMENT Village (MunicipalityCode,VillageCode,                   |
      |    VillageName,MalePopulation ?, FemalePopulation ?,                  |
      |    OtherPopulation,Families ?)>                                       |
      |                                                                       |
      |    < !ELEMENT MunicipalityCode (#CDATA)>                              |
      |                                                                       |
      |    < !ELEMENT VillageCode (#CDATA)>                                   |
      |                                                                       |
      |    < !ELEMENT VillageName (#CDATA)>                                   |
      |                                                                       |
      |    < !ELEMENT MalePopulation (#CDATA)>                                |
      |                                                                       |
      |    < !ELEMENT FemalePopulation (#CDATA)>                              |
      |                                                                       |
      |    < !ELEMENT OtherPopulation (#CDATA)>                               |
      |                                                                       |
      |    < !ELEMENT Families (#CDATA)>                                      |
      |                                                                       |
      |    ]>                                                                 |
      +-----------------------------------------------------------------------+

  C. Upload of the register of health facilities

    * ``Browse``

      Select from a file in the XML format serving as a source for uploading of the register of health facilities. Mandatory.

    * ``Strategy``

      Select a desired strategy for uploading of the register of health facilities. The following options are available:

    * ``Insert Only``

      Uploads only health facilities that are not yet included in the register of health facilities

    * ``Update Only``

      Updates only health facilities that are already included in the register of health facilities

    * ``Insert and Update``

      Uploads health facilities that are not yet included in the register of health facilities and updates health facilities that are already included in the register of health facilities

    * ``Dry Run``

      If checked only diagnostics is provided without real uploading.

    * ``Upload``

      By clicking on the Upload button, a prompt popup message will appear, require a user to agree or disagree: (:ref:`image_upload_facilities`) If user agrees the selected file containing locations will be uploaded.

      .. _image_upload_facilities:
      .. figure:: /img/user_manual/image_upload_facilities.png
        :align: center

        `Upload Health Facilities`

      A statistics on the number of inserted/updated health facilities
      appears.

      If there are errors an error protocol appears.

      +-----------------------------------------------------------------------+
      | *DTD definition of the XML file for uploading/downloading of health   |
      | facilities:*                                                          |
      |                                                                       |
      |    <!DOCTYPE HealthFacilities> [                                      |
      |                                                                       |
      |    <!ELEMENT HealthFacilities                                         |
      |    (HealthFacilityDetails,CatchmentsDetails)>                         |
      |                                                                       |
      |    <!ELEMENT HealthFacilityDetails (HealthFacility)*>                 |
      |                                                                       |
      |    <!ELEMENT HealthFacility (LegalForm, Level, Sublevel, Code, Name,  |
      |    Address, DistrictCode, DistrictName, Phone, Fax, Email, CareType,  |
      |    AccountCode, ItemPriceListName. ServicePricelistName)>             |
      |                                                                       |
      |    <!ELEMENT LegalForm (D\| C|G|P)>                                   |
      |                                                                       |
      |    <!ELEMENT Level (D|C|H)>                                           |
      |                                                                       |
      |    <!ELEMENT SubLevel (I|N|R)>                                        |
      |                                                                       |
      |    <!ELEMENT Code (#CDATA)>                                           |
      |                                                                       |
      |    <!ELEMENT Name (#CDATA)>                                           |
      |                                                                       |
      |    <!ELEMENT Address (#CDATA)>                                        |
      |                                                                       |
      |    <!ELEMENT DistrictCode (#CDATA)>                                   |
      |                                                                       |
      |    <!ELEMENT DistrictName (#CDATA)>                                   |
      |                                                                       |
      |    <!ELEMENT Phone (#CDATA)>                                          |
      |                                                                       |
      |    <!ELEMENT Fax (#CDATA)>                                            |
      |                                                                       |
      |    <!ELEMENT Email (#CDATA)>                                          |
      |                                                                       |
      |    <!ELEMENT CareType (I|N|B)>                                        |
      |                                                                       |
      |    <!ELEMENT AccountCode (#CDATA)>                                    |
      |                                                                       |
      |    <!ELEMENT ItemPriceListName (#CDATA)>                              |
      |                                                                       |
      |    <!ELEMENT ServicePriceListName (#CDATA)>                           |
      |                                                                       |
      |    <!ELEMENT CatchmentsDetails(Catchment*)>                           |
      |                                                                       |
      |    <!ELEMENT Catchment (HFCode,VillageCode, VillageName, Percentage)> |
      |                                                                       |
      |    <!ELEMENT HFCode (#CDATA)>                                         |
      |                                                                       |
      |    <!ELEMENT VillageCode (#CDATA)>                                    |
      |                                                                       |
      |    <!ELEMENT VillageName (#CDATA)>                                    |
      |                                                                       |
      |    <!ELEMENT Percentage (#CDATA)>                                     |
      |                                                                       |
      |    ]>                                                                 |
      +-----------------------------------------------------------------------+

  D. Download of the list diagnoses

    * ``Download``

      By clicking on the Download button, a prompt popup message will appear, require a user to specify whether the XML file with downloaded list of diagnoses should be opened or saved or canceled: (:ref:`image_download_diagnoses`)

      .. _image_download_diagnoses:
      .. figure:: /img/user_manual/image_download_diagnoses.png
        :align: center

        `Download Diagnoses`

  E. Download of the register of locations

    * ``Download``

      By clicking on the Download button, a prompt popup message will appear, require a user to specify whether the XML file with downloaded register of locations should be opened or saved or canceled (:ref:`image_download_locations`)

      .. _image_download_locations:
      .. figure:: /img/user_manual/image_download_locations.png
        :align: center

        `Download locations`

  F. Download of the register of health facilities

    * ``Download``

      By clicking on the Download button, a prompt popup message will appear, require a user to specify whether the XML file with downloaded  canceled (:ref:`image_download_facilities`)

      .. _image_download_facilities:
      .. figure:: /img/user_manual/image_download_facilities.png
        :align: center

        `Download facilities`

  G. Buttons

  * ``Cancel``

    By clicking on ``Cancel`` button, user will be re-directed to the Home
    page.

  H. Information Panel

    The Information Panel is used to display messages back to the user.
