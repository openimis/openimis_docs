
Web application user manual
===========================

  **v1.2.1**

  The open Insurance Management Information System ( openIMIS ) is a web based software to manage health insurance schemes. It includes functionality for setup of the software to requirements of health insurance schemes, administration of policies and policy holders and for claim processing. This manual is a guide on the use and functionality of the software rather than in-depth technical reference. The Contents section, provide a reference to the page of each major chapter and the sub chapters within. By clicking on the content title (online version), the reader is re-directed to the position of the content title.

  .. The following conventions are used:
    - `<Hyperlink>`_  enable a quick link (using the online version) to the subject relating to the functionality,
    - **Item** means an item in a drop down list,
    - ``LABEL`` means a data field or a button,
    - _NAME_OF_PAGE_ means a name of page or a data field in a text without hyperlink.


Users and logins
----------------

.. include:: /_include/um/user_login/login.rst
.. include:: /_include/um/user_login/forgotten_password.rst
.. include:: /_include/um/user_login/password_change.rst

Administration of registers
---------------------------

  Registers of openIMIS serve as a principal tool by which openIMIS is adjusted to needs of health insurance schemes. With exception of the register of Users that can be managed only by users with the role openIMIS Administrator, all other registers can be managed by users with the role Scheme Administrator.

  The register of Users defines who can login to openIMIS and under what constraints. The register of Locations defines administrative division of the territory, on which a health insurance scheme is operated. The register of Payers allows specification of institutional payers that can pay contributions on behalf of policy holders (households, groups of persons). The register of Enrolment Agents specifies all persons (either employed or contracted) by the scheme administration that are entitled to distribute/sell policies to population. The register of Claim Administrators specifies all employees of health facilities that are entitled to submit claims to the scheme administration. The register of Health Facilities contains all contractual health facilities that can submit claims to the scheme administration. The register of Medical Items specifies all possible medical items (drugs, prostheses, medical devices etc.) that can be used in definitions of packages of insurance products and in pricelists associated with contractual health facilities. The register of Pricelists that splits into two divisions for Medical Services and for Medical Items contains pricelists valid for individual health facilities or their groups reflecting results of price negotiations between contractual health facilities and the scheme administration. Finally, the register of Products includes definitions of all insurance products that can be distributed/ sold within the health insurance scheme.

.. include:: /_include/um/register/policy.rst
.. include:: /_include/um/register/health_facility.rst
.. include:: /_include/um/register/medical_service.rst
.. include:: /_include/um/register/medical_item.rst
.. include:: /_include/um/register/service_price_list.rst
.. include:: /_include/um/register/item_price_list.rst
.. include:: /_include/um/register/user.rst
.. include:: /_include/um/register/user_roles.rst
.. include:: /_include/um/register/enrolment_officer.rst
.. include:: /_include/um/register/claim_admin.rst
.. include:: /_include/um/register/payer.rst
.. include:: /_include/um/register/location.rst

Insurees and Policies
---------------------

.. include:: /_include/um/insuree_policies/quick_find_insuree.rst
.. include:: /_include/um/insuree_policies/find_family.rst
.. include:: /_include/um/insuree_policies/find_insuree.rst
.. include:: /_include/um/insuree_policies/find_policy.rst
.. include:: /_include/um/insuree_policies/find_contribution.rst
.. include:: /_include/um/insuree_policies/family_overview.rst

Claims
------

  The functionality under the menu ``Claims`` allows complete processing of claims from their entering into IMIS, modification, submission to processing, automatic checking of their correctness, reviewing of them by medical officers, their evaluating and preparation of report to an accounting system for their remuneration to contractual health facilities. Each claim can be consequently in several states. Once it is entered to openIMIS (either by the mobile phone application **Claim Management** or typed in and saved in IMIS) it goes to the status **Entered**. When it is submitted and it successfully passes at least some automatic checks, the claim goes to the status **Checked**. If the claim doesn’t pass automatic checking it goes to the status **Rejected** and its processing ends. The claim in the status **Checked** may be reviewed from medical point of view and/or a feedback on it can be collected from the patient. Medical reviewing and feedback acquiring can be by-passed. Ones such (manual) scrutiny of the claim is at the end, the claim may be pushed to the status **Processed**. In this status the claim is evaluated in nominal prices, taking into account all ceilings, deductibles and other cost sharing rules associated with insurance product or products covering claimed health care. If there is no medical service or medical item price of which a relative one according to the corresponding insurance product, the claim goes automatically to the status **Valuated**. If there is at least one medical service or medical item with relative pricing, the claim goes to the status **Valuated** only after a batch for corresponding period is run. The batch for a period (month, quarter, year) finishes evaluation of relative prices on claims on one hand and summarizes all claims in the period for accounting system that is external to openIMIS (it is not a part of it). Different values (prices) of a claim are associated with each stage of processing of claims. When a claim is entered the value of the claim based on nominal prices of claimed medical services/items is designated as **Claimed Value**. **Claimed Value** is associated with the state **Entered**. The value of the claim after automatic checking of claims during submission of the claim and after manual interventions of medical officers is designated as **Approved Value**. **Approved Value** is associated with the state **Checked**. The value of the claim after corrections based on all cost sharing rules of covering insurance products is designated as **Adjusted Value**. **Adjusted Value** is associated with the state **Processed**. The final value of the claim taking into account actual value of relative prices is designated as **Paid Value**. **Paid Value** is associated with the state **Valuated**.

.. include:: /_include/um/claims/hf_claims.rst
.. include:: /_include/um/claims/review_claims.rst
.. include:: /_include/um/claims/batch_claims.rst

Tools
-----

Upload / Download selected registers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  Access to uploading/downloading of selected registers is restricted to the users with the role of openIMIS Administrator.

Navigation
""""""""""

  All functionality for use with the administration of uploading/downloading of selected registers can be found under the main menu ``Tools``, sub menu ``Registers``.

  .. _image166:
  .. figure:: /img/user_manual/image136.jpeg
    :align: center

    `Image 166 - Navigation to Registers`

  Clicking on the sub menu ``Registers`` re-directs the current user to the `Registers Page`: (:ref:`Image 166<image166>`)

Registers page
""""""""""""""

  .. _image167:
  .. figure:: /img/user_manual/image137.jpeg
    :align: center

    `Image 167 - Upload Registers`

  The Registers Page is divided into eight sections: (:ref:`Image 167<image167>`)

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

Policy Renewals
^^^^^^^^^^^^^^^

  Access to management of policy renewals is restricted to the users with the role of Clerk.

Navigation
""""""""""

  All functionality for use with the administration of policy renewals can be found under the main menu ``Tools``, sub menu ``Policy Renewals``

  .. _image169:
  .. figure:: /img/user_manual/image139.png
    :align: center

    `Image 169 - Navigation Policy Renewals`

  Clicking on the sub menu ``Policy Renewals`` re=directs the current user to the `Policy Renewal Page <#policy-renewal-page>`__\.

  .. _image170:
  .. figure:: /img/user_manual/image140.png
    :align: center

    `Image 170 - Policy Renewal Page`

Policy Renewal Page
"""""""""""""""""""

  By having access to this page, it is possible preview the report on policy renewals, preview the journal on policy renewals and update the status of a policy. The journal will contain information on actual prompts being generated by the system. These prompt could already have been sent to the mobile phones of enrolment officers. The report on policy renewals will contain information on the expiration of policies for any given period. The page is divided into two panels (:ref:`Image 170<image170>`).

 #. **Select Criteria Panel**

    The Select Criteria Panel or the filter panel allows a user to select specific criteria to minimise the report on policy renewals.

    Two tasks are carried out by this form. 1) Preview the report on policy renewal and 2) Preview the journal on policy renewal. Depending on the selected option, filter will be changed accordingly.

    If Preview option is selected then a user has the following filters.

    * ``Policy Status``

      Select the policy status from the drop down list by clicking on the right arrow. By selecting any of the options a user can filter the report on particular status of the policy. This filter is not mandatory. User can leave it blank to preview the report on any status.

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select policies from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected.*

    * ``District``

      Select the ``district``; from the list of districts by clicking on the arrow on the right of the selector to select policies from a specific district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected.*

    * ``Municipality``

      Select the ``Municipality``; from the list of municipalities by clicking on the arrow on the right of the selector to preview report from a specific district. *Note: The list will only be filled with the municipalities that belong to the selected district. If this is only one then the municipality will be automatically selected.*

    * ``Village``

      Select the ``village``; from the list of villages by clicking on the arrow on the right of the selector to preview report from a specific village. *Note: The list will only be filled with the villages that belong to the selected municipality.*

    * ``Enrolment Officer``

      Select the ``Enrolment Officer``; from the list of enrolment officers by clicking on the arrow on the right of the selector to preview the report for the specific officer. *Note: The list will only be filled with the enrolment officers belonging to the districts assigned to the current logged in user. If this is only one then the enrolment officer will be automatically selected.*

    * ``Date From``

      By clicking on the button next to the ``Date From`` data field a calendar will pop up. Click on his desired date and the textbox will be filled with the selected date. This is a mandatory field. Only the policies for renewal date greater than or equal to the ``Date From`` will be previewed.

    * ``Date To``

      By clicking on the button next to the ``Date To`` data field a calendar will pop up. Click on his desired date and the textbox will be filled with the selected date. This is a mandatory field. Only the policies for renewal date less than or equal to the ``Date To`` will be previewed.

      When previewing the journal; the ``Policy Status`` filter will be replaced with ``SMS Status`` and there will be one more additional filter, ``Journal On``.

    * ``SMS Status``

      Select the ``SMS status`` from the drop down list by clicking on the right arrow. By selecting any of the options the user can filter the journal on a particular ``SMS status``. This filter is not mandatory. By leaving it blank all journals will be displayed.

    * ``Journal On``

      Select the ``journal On`` from the drop down *list* by clicking on the right arrow, to filter the journal either on prompt or on expiry of the prompt.

 #. **Button Panel**

    ``Cancel:`` Re-directs to the `Home Page <#image-2.2-home-page>`__

    ``Preview:`` Click on the preview button to display the report based on the filters.

    ``Update:`` Click on this button to manually update the status of the policy on the current day. Although this task is carried out by the **IMIS Policy Renewal Service** running on the server at specific intervals of time, this button enables the task to be run manually.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a user has updated the policy status or if there was an error at any time during the process of these actions.

Preview Report on Renewals
""""""""""""""""""""""""""

  .. _image172:
  .. figure:: /img/user_manual/image142.png
    :align: center

    `Image 172 - Preview Report on Renewals`

  After selecting specific criteria; preview the report (:ref:`Image 172<image172>`) by clicking on the preview button.

Preview Journal on Renewals
"""""""""""""""""""""""""""

  Just like preview of the policy renewals the journal report can also be previewed. The difference between the Policy Renewal report and the Journal is; one forecasts the renewal while the other gives a report on the status of the renewal. Below is an example of a Journal Report.

  .. _image173:
  .. figure:: /img/user_manual/image143.png
    :align: center

    `Image 173 - Preview Journal on Renewals`

Feedback Prompts
^^^^^^^^^^^^^^^^

  Access to administration of feedback prompts is restricted to the users with the role of Medical Officer.

Navigation
""""""""""

  All functionality for use with the administration of feedback prompt can be found under the main menu ``Tools``, sub menu ``Feedback Prompts``

  .. _image174:
  .. figure:: /img/user_manual/image144.png
    :align: center

    `Image 174 - Navigation Feedback Prompts`

  Clicking on the sub menu ``Feedback Prompts`` re-directs the current user to the Feedback Prompt Page (:ref:`Image 174<image174>`).

  .. _image175:
  .. figure:: /img/user_manual/image145.png
    :align: center

    `Image 175 - Feedback Prompts Page`

  The Feedback Prompt Page is divided into three panels (:ref:`Image 175<image175>`).

 #. **Select Criteria Panel**

    The Select Criteria Panel or the filter panel allows a user to select specific criteria for feedback.

    * ``SMS Status``

      Select ``SMS Status`` from the list

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select a specific region for feedbacks. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected.*

    * ``District``

      Select the ``district`` from the list of districts by clicking on the arrow on the right of the selector to select district for feedbacks. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the District will be automatically selected.*

    * ``Municipality``

      Select the ``Municipality`` from the list of municipalities you wish to prompt for feedbacks. *Note: The list will only be filled with the municipalities that belong to the selected district. If this is only one then the municipality will be automatically selected.*

    * ``Village``

      Select the ``village``; from the list of villages you wish to prompt for feedbacks. *Note: The list will only be filled with the villages that belong to the selected municipality.*

    * ``Enrolment Officer``

      Select the ``Enrolment Officer``; from the list of enrolment officers by clicking on the arrow on the right of the selector to preview the report for the specific officer. *Note: The list will only be filled with the enrolment officers belonging to the districts assigned to the current logged in user. If this is only one then the enrolment officer will be automatically selected.*

    * ``Start Date``

      Type in a date; or use the Date Selector Button, to enter the ``Start Date`` for feedbacks. *Mandatory. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``End Date``

      Type in a date; or use the Date Selector Button, to enter the ``End Date`` for feedbacks. *Mandatory*. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Send SMS``

      By Clicking ``Send SMS`` button, user actually sends an SMS. When an SMS is sent successfully as message will be given. If failed to be sent, a failure message will appear.

 #. **Buttons Panel**

    * ``Preview``

      By clicking on the ``Preview`` button, a report (journal) of feedbacks prompted will get generated and displayed (:ref:`Image 176<image176>`).

    * ``Cancel``

      By clicking on ``Cancel`` button, user will be re-directed to `Home Page <#image-2.2-home-page>`__.

      .. _image176:
      .. figure:: /img/user_manual/image146.png
        :align: center

        `Image 176 - Feedback Prompt Journal`

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur if there was an error at any time during the processing of the reports.

IMIS Extracts
^^^^^^^^^^^^^

  Access to the openIMIS Extracts page is restricted to users with the role of Scheme Administrator (IMIS Central online) or HF Administrator (offline installations). This page will contain all functionality for data synchronization between openIMIS Central and openIMIS offline installations as well as the generation of extract files for the mobile phones (Android). Depending on the type of installation, the interface will enable and disable certain functions.

Pre-conditions
""""""""""""""

  The extract functionality is covering extracts for the mobile phone applications and the openIMIS ‘offline’ installations. Offline extracts are only to be generated in case a district has so called ‘off-line’ installations in areas where no Internet connectivity is available.

  Extracts are to be downloaded to the local PC that is initiating the creation of the extract.

  Standard procedures should be formulated to stipulate the time interval between Extract creations and the management of transporting and installing/transferring these extracts into the target environment: mobile phones or offline openIMIS clients.

Navigation
""""""""""

  All functionality related to openIMIS extracts can be found under the main menu ``Tools``, sub menu ``IMIS Extracts``

  .. _image177:
  .. figure:: /img/user_manual/image147.png
    :align: center

    `Image 177 - Navigation openIMIS Extracts`

  Clicking on the sub menu ``IMIS Extracts`` re-directs the current user to the ``IMIS Extracts Page.``

  This page opens in two different modes depending on the type of openIMIS installation: openIMIS Central (live server) or openIMIS offline (installed on local network in a health facility or an office of the scheme administration).

IMIS Extracts (online mode)
"""""""""""""""""""""""""""

  .. _image178:
  .. figure:: /img/user_manual/image148.jpeg
    :align: center

    `Image 178 - openIMIS Extracts`

  The Extracts Page is divided into eight sections `(Image
  6.23) <#image-6.2-registers-page>`__\ \ .

  **A - Download Master Data section**

The Master Data section is used for generation of the data needed for off-line operation of IMIS (Policies) application run on Android platforms. The following data files can be downloaded:

    - Master data for running IMIS (Policies) application **(Download Master Data)**

    - Prompts for renewal of policies **(Download Renewals)**

    - Prompts for acquiring of feedbacks **(Download Feedbacks)**

    - **Enrolment Officers Code**: Enter the code of an enrolment officer for whom the master data and prompts should be generated.

  **B - Create Phone Extract section**

  The Phone extract panel is used for the generation of so called SQLite database files for the mobile phone applications. Each district will have its own phone extract file that needs to be distributed to the mobile phones within the district. To generate a phone extract file, the operator has to select a region and a district from the list of available districts. In case the user is having access to its own district only, the district will be automatically selected and shown on the display.

  By clicking the ``Create`` button in panel the section, a phone extract will be created. This process might take a while. As long as the hour glass (as a cursor) is shown, openIMIS is still processing the file. The file size depends on the amount of photographs included in the extract. The file size could range into hundreds of MBs. To alleviate this problem two options are available:

    * ``With Insurees``

      Checking this box means that a complete phone extract (including photos) will be generated. Leaving it unchecked a shortened phone extract without photos will be generated.

    * ``In background``

      Checking this box means that the phone extract will be created in background and the user will be notified by e-mail (provided his/her e-mail is entered in the register of users).

    In case the extract is created in the background, the following dialog box appears:

    .. _image179:
    .. figure:: /img/user_manual/image149.png
      :align: center

      `Image 179`

    If the extract is not created in background the user is notified about successful creation by the following message as shown below.

    .. _image180:
    .. figure:: /img/user_manual/image150.png
      :align: center

      `Image 180`

    The extract will be downloaded to your local computer by clicking the ``Download`` link that will appear after the creation of the extract, as shown below.

    .. _image181:
    .. figure:: /img/user_manual/image151.png
      :align: center

      `Image 181`

    The extract file is called **IMISDATA.DB3** and needs first to be copied (downloaded) to the local machine. After clicking the ``Download`` button, the operator is able to select the destination folder (locally) for the file to download as shown below.

    .. _image182:
    .. figure:: /img/user_manual/image152.png
      :align: center

      `Image 182`

    The extract is now ready to be transferred/copied to the mobile phones. This process is performed manually by connecting the mobile phone to the computer with the provided USB cable. The user needs to copy, manually, the file from the local machine into the ‘IMIS’ Folder on the mobile phone.

  **C - Offline Extract section**

  The offline extract section is used to generate the openIMIS ‘offline’ extract files for the health facilities or offices of the scheme administration that run openIMIS offline. To generate an offline extract file, the operator has to select a region and a district from the list of available districts. In case the user is having access to its own district only, the district will be automatically selected and shown on the display. When an operator belongs to one specific district, the district box is already selected with the district of the user. To create a new extract, the operator needs to click the ``Create`` button.

  Three types of extracts could be generated:

      - Differential Extract ``(Download D)``

        Differential extracts will only contain the differences in data compared with the previous extract. The first differential extract (sequence 000001) will contain all data as it will be the first extract. Thereafter, this type of the extract, will only contain any differences after the previous extract. This will result in smaller files sent to the health facilities in off-line mode. When we click the create button, the differential extract is always generated and will be assigned the next sequence number. A separate Photo extract will be created containing only photographs linked to changes compared with the previous extract. Differential extracts with insure and policy data are only generated in case the ``With Insuree`` checkbox is checked as shown below.

        .. _image183:
        .. figure:: /img/user_manual/image153.png
          :align: center

          `Image 183`

      - Full extract ``(Download F)``

        The Full extract will always contain all information in the database. These extracts are only generated in case the ``Full extract`` and the ``With Insuree`` checkbox are checked as shown below.

        .. _image184:
        .. figure:: /img/user_manual/image154.png
          :align: center

          `Image 184`

        By clicking the ``Create`` button, in case of ``Full extract`` is checked, two extracts will be generated, one differential extract and one full extract. Both extracts will have the same sequence number. This implies that full extracts are not always needed/generated. A separate photo extract will be created containing all photographs.

      - Empty Extract ``(Download E)``

        Empty extracts will only contain the data from registers and no data on insurees and their policies/photos. If a full set of register data should be included in the extract, the checkbox ``Full extract`` has to be checked as shown below.

        .. _image185:
        .. figure:: /img/user_manual/image155.png
          :align: center

          `Image  185`

  After clicking the ``Create`` button, the system will create the extract file and will on completion display the following message:

  .. _image186:
  .. figure:: /img/user_manual/image156.png
    :align: center

    `Image 186`

  The message is only shown to provide some details on how much information is exported to the extract file.

  Depending on the ``Full extract`` option, we will be re-directed to the extract page and will see the newly generated extract sequence in the list or will get a new message as shown below:

  .. _image187:
  .. figure:: /img/user_manual/image157.png
    :align: center

    `Image 187`

  After clicking OK the statistics of the full extract will be shown:

  .. _image188:
  .. figure:: /img/user_manual/image158.png
    :align: center

    `Image 188`

  We are now ready to download the extract to our computer.

  The combo box next to the district selector contains information on all generated extracts with the sequence number and date. (e.g. Sequence 000007 – Date 06-09-2012). If the extract selector does not show any entries (blank) it means that no previous extracts were created. At least one full extract needs to be generated. This is needed to initialise a new offline openIMIS installation.

  To download the actual extracts, the operator needs to select the desired extract sequence from the list of available extracts.

  Four different types of extracts could be downloaded by clicking one of the following buttons:

    * ``Download D`` (Differential extract)

      - Will download the selected differential extract with the following filename

        *Filename: OE_D_<DistrictID>_<Sequence>.RAR (e.g. OE_D_1_8.RAR)*

    * ``Download F`` (Full extract)

      - Will download the latest full extract with the following filename

        *Filename: OE_F_<DistrictID>_<Sequence>.RAR (e.g. OE_F_1_8.RAR)*

    * ``Download E`` (Empty extract)

      - Will download the latest full extract with the following filename

        *Filename: OE_E_<DistrictID>_<Sequence>.RAR (e.g. OE_F_1_8.RAR)*

    * ``Download Photos D`` (Differential Photo extract)

      - Will download the selected differential photo extract with filename:

        *Filename: OE_D_<DistrictID>_<Sequence>.RAR (e.g. OE_D_1_8_Photos.RAR)*

    * ``Download Photos F`` (Full Photo extract)

      - Will download the latest FULL photo extract with the following filename

        *Filename: OE_D_<DistrictID>_<Sequence>.RAR (e.g. OE_F_1_8_Photos.RAR)*

  After clicking the desired extract download button, the file download dialog box appears to select the destination folder for the extract file as shown below:

  .. _image189:
  .. figure:: /img/user_manual/image159.png
    :align: center

    `Image 189`

  In case the extract file is not available (anymore) on the server, the following dialog box might appear:

  .. _image190:
  .. figure:: /img/user_manual/image160.png
    :align: center

    `Image 190`

  The reason for this box to appear could be that the file to be downloaded has been removed from the server or that you have attempted the download a full extract but no full extract was generated (only the differential extracts exist). It is also possible that you have attempted to download a photo extract but no photos were added since the last extract.

  Checking the checkbox ``In background`` means that the off-line extract will be created in background and the user will be notified by e-mail (provided his/her e-mail is entered in the register of users) as shown below:

  .. _image191:
  .. figure:: /img/user_manual/image161.png
    :align: center

    `Image 191`

  In case the extract is created in the background, the following dialog box appears:

  .. _image192:
  .. figure:: /img/user_manual/image149.png
    :align: center

    `Image 192`

  **D - Upload Claims section**

    - **Browse**

      Browse for the file from the IMIS-Offline or IMIS (Claims )
      application containing claims to be uploaded.

    - Upload

      Upload claims contained in the selected file.

  **E - Upload Enrolment section**

    - **Browse**

      Browse for the file from the IMIS-Offline or IMIS (Policies
      )application containing newly enrolled or renewed policies to be
      uploaded.

    - Upload

      Upload policies contained in the selected file.

  **F - Upload Feedback section**

    - **Browse**

      Browse for the file from the IMIS-Offline or IMIS (Policies
      )application containing feedbacks to be uploaded.

    - Upload

      Upload feedbacks contained in the selected file.

  **G - Button section**

  The ``Cancel`` button brings the operator back to the `Home Page <#image-2.2-home-page>`__.

  **H - Information panel**

  The Information Panel is used to display messages back to the user. Messages will occur once an action has completed or if there was an error at any time during the process of these actions.

IMIS Extracts (OFFLINE MODE)
""""""""""""""""""""""""""""

  **Offline HF**

  .. _image193:
  .. figure:: /img/user_manual/image162.png
    :align: center

    `Image 193`

  **A - Import Extract**

  Used to extract photos obtained from online IMIS

  **B - Import Photos**

  Used to upload photos obtained from online IMIS

  **C - Download Claim XMLs**

  Used to download claims made in the offline health facility prior to be sent to online IMIS

  **Offline Insurer**

  .. _image194:
  .. figure:: /img/user_manual/image163.png
    :align: center

    `Image 194`

  **A - Import Extract**

  Used to upload extract obtained from online IMIS

  **B - Import Photos**

  Used to upload photos obtained from online IMIS

  **C - Import Extract**

  The Choose file section should be clicked to select an extract file to upload/import. The following file selector appears for Internet explorer (the appearance might differ for different internet browsers):

  .. _image195:
  .. figure:: /img/user_manual/image164.png
    :align: center

    `Image 195`

  On clicking the ``Choose File`` button, the file selector dialog appears as shown below:

  .. _image196:
  .. figure:: /img/user_manual/image165.png
    :align: center

    `Image 196`

  With the import/upload of an extract it is important to understand that each extract has its sequence number. This sequence number is found in the filename of the extract. We would in case of differential imports/uploads have to follow the sequence. In the example screen above, it shows in the status bar, that the last import was number 6. Therefore we should select in this case the differential extract number 7 as highlighted in the file selection dialog.

  Alternatively the operator could select any full extract with a sequence number higher than 6. In case a wrong extract is selected, warning messages will appear as shown below:

  .. _image197:
  .. figure:: /img/user_manual/image166.png
    :align: center

    `Image 197`

  .. _image198:
  .. figure:: /img/user_manual/image167.png
    :align: center

    `Image 198`

  In case you are missing extract sequences, additional extracts are needed to be uploaded before the extract selected. The extract selected, in this case, does not directly follow the last sequence as indicated in the status bar of the screen. The additional extracts are to be provided by NSHIP district office.

  In case the extract file selected is valid, the system will import the data. New data will be added and existing data might be modified. After a successful import of an extract (Differential and FULL), a form is displayed with the statistics of the import as shown below:

  .. _image199:
  .. figure:: /img/user_manual/image168.png
    :align: center

    `Image 199`

  The above statistics are provided to give some quick overview of how many records were inserted or updated during the import process. In case we would for example update the phone number of an enrolment officer, it would result in one update and one insert as we always keep historical records. The photos inserts and updates are related to information on the photos, but are not the actual photographs. The actual photographs (\\*.jpg) are uploaded separately.

  **D - Import Photos**

  The import of photos is optional and will have no further checking on sequence numbers. NSHIP should provide (if available) with each extract the photo extract as well.

  E.g. (for Differential extract)

  .. _image200:
  .. figure:: /img/user_manual/image169.png
    :align: center

    `Image 200`

  OR (for FULL extract)

  .. _image201:
  .. figure:: /img/user_manual/image170.png
    :align: center

    `Image 201`

  The photo extract will contain all photographs associated with the actual extract in a zipped format. The Upload procedure will simply unzip the extract and copy the image files to the photo folder of IMIS.

  After successful upload of the photographs the following message appears:

  .. _image202:
  .. figure:: /img/user_manual/image171.png
    :align: center

    `Image 202`

  **E - Button panel**

  The ‘Cancel’ button brings the operator back to the main page of IMIS.

  **F - Information panel**

  The Information Panel is used to display messages back to the user. Messages will occur once an action has completed or if there was an error at any time during the process of these actions. If the user opens the openIMIS extracts page (in offline mode only), the status bar will show the last sequence number uploaded.

Reports
^^^^^^^

  Access to the reports is generally restricted to the users with the role of Manager, Accountant, Scheme Administrator and openIMIS Administrator. By having access to the ``Reports Page``, it is possible to generate several operational reports. Each report can be generated by users with a specific role (Manager, Accountant, Scheme Administrator and openIMIS Administrator) only.

Pre-Conditions
""""""""""""""

Navigation
"""""""""""

  All functionality for use with the administration of Reports can be found under the main menu ``Tools``, sub menu ``Reports.``

  .. _image203:
  .. figure:: /img/user_manual/image172.png
    :align: center

    `Image 203 - Navigation Reports`

  Clicking on the sub menu ``Reports`` re-directs the current user to the Reports Page (:ref:`Image 204<image204>`).

  .. _image204:
  .. figure:: /img/user_manual/image173.png
    :align: center

    `Image 204 - Reports Page`

  The Reports Page is divided into four panels (:ref:`Image 204<image204>`).

 #. **Select Criteria**

    The Select Criteria panel or the filter panel allows a user to select specific criteria determining the scope of data included in the report. The criteria (:ref:`Image 205<image205>` – :ref:`Image 222<image222>`) will change depending on the selected type of the report.

      - Primary Operational Indicators - Policies Report.

      .. _image205:
      .. figure:: /img/user_manual/image174.png
        :align: center

        `Image 205 - Primary Operational Indicators - Policies Report Criteria`

      - Primary Operational Indicators - Claims Report.

      .. _image206:
      .. figure:: /img/user_manual/image175.png
        :align: center

        `Image 206 - Primary Operational Indicators - Claims Report Criteria`

      - Derived Operational Indicators Report.

      .. _image207:
      .. figure:: /img/user_manual/image176.png
        :align: center

        `Image 207 - Derived Operational Indicators Report Criteria`

      - Contribution Collection Report.

      .. _image208:
      .. figure:: /img/user_manual/image177.png
        :align: center

        `Image 208 - Contribution Collection Report Criteria`

      - Product Sales Report.

      .. _image209:
      .. figure:: /img/user_manual/image178.png
        :align: center

        `Image 209 - Product Sales Report Criteria`

      - Contribution Distribution Report.

      .. _image210:
      .. figure:: /img/user_manual/image179.png
        :align: center

        `Image 210 - Contribution Distribution Report Criteria`

      - User Activity Report.

      .. _image211:
      .. figure:: /img/user_manual/image180.png
        :align: center

        `Image 211 - User Activity Report Criteria`

      - Enrolment Performance Indicator Report.

      .. _image212:
      .. figure:: /img/user_manual/image181.png
        :align: center

        `Image 212 - Enrolment Performance Indicators Report Criteria`

      - Status of Registers Report.

      .. _image213:
      .. figure:: /img/user_manual/image182.png
        :align: center

        `Image 213 - Status of Registers Report Criteria`

      - Insurees without Photos Report.

      .. _image214:
      .. figure:: /img/user_manual/image183.png
        :align: center

        `Image 214 - Insurees without photos Report Criteria`

      - Payment Category Overview Report.

      .. _image215:
      .. figure:: /img/user_manual/image184.png
        :align: center

        `Image 215 - Payment Category Overview Report Criteria`

      - Matching Funds Report.

      .. _image216:
      .. figure:: /img/user_manual/image185.png
        :align: center

        `Image 216 - Matching funds Report Criteria`

      - Claim Overview Report.

      .. _image217:
      .. figure:: /img/user_manual/image186.png
        :align: center

        `Image 217 - Claim Overview Report Criteria`

      - Percentage of Referrals Report.

      .. _image218:
      .. figure:: /img/user_manual/image187.png
        :align: center

        `Image 218 - Percentage of Referrals Report Criteria`

      - Families and Insurees Overview Report.

      .. _image219:
      .. figure:: /img/user_manual/image188.png
        :align: center

        `Image 219 - Families and Insurees Overview Report Criteria`

      - Pending Insurees Report.

      .. _image220:
      .. figure:: /img/user_manual/image189.png
        :align: center

        `Image 220 - Pending Insurees Report Criteria`

      - Renewals Report.

      .. _image221:
      .. figure:: /img/user_manual/image190.png
        :align: center

        `Image 221 Renewals Report Criteria`

      - Capitation Payment Report

      .. _image222:
      .. figure:: /img/user_manual/image191.png
        :align: center

        `Image 222 Capitation Payment Report Criteria`

  The general meaning of selection criteria for creating of a report is as follows:

    * ``Date From``

      Type in a date; or use the Date Selector Button, to enter the beginning of a period, in which policies have their enrolment, effective, expire or renewal days, contributions were paid or in claimed health care was provided. If used with a report, it is mandatory. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Date To``

      Type in a date; or use the Date Selector Button, to enter the end of a period, in which policies have their enrolment, effective, expire or renewal days or in which claimed health care was provided. If used with a report, it is mandatory. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Payment Type``

      Select the ``Payment Type`` from the drop down list by clicking on the right arrow. By selecting any of the options a user can filter the report on a particular type of the payment. This filter is not mandatory, leave it blank to preview the report on all the payment modes.

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select a region, data of which should be included for the report. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected.*

    * ``District``

      Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to select a district, data of which should be included for the report. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected.*

    * ``Product``

      Select the ``Product``; from the list of products by clicking on the arrow on the right of the selector to include in the report data for the specific product. *Note: The list will only be filled with the products belong to the districts assigned to the current logged in user. If this is only one then the product will be automatically selected.*

    * ``Month``

      Select the ``Month`` from the list of months by clicking on the arrow on the right of the selector to include in the report data relating to that month selected.

    * ``Year``

      Select the ``year`` from the list of years by clicking on the arrow on the right of the selector to include in the report data relating to that year selected.

    * ``Quarter``

      Select the ``quarter`` from the list of quarters by clicking on the arrow on the right of the selector to include in the report data relating to that quarter selected.

    * ``HF Code``

      Select the ``HF Code``; from the list of heath facility codes by clicking on the arrow on the right of the selector to create the report for the specific health facility. *Note: The list will only be filled with health facility codes of health facilities belonging to the districts assigned to the current logged in user. If this is only one then the health facility code will be automatically selected.*

    * ``Enrolment Officer``

      Select the enrolment officer; from the list of enrolment officers by clicking on the arrow on the right of the selector to select enrolment officer data of whom should be included in the report. *Note: The list will only be filled with the enrolment officers assigned to the current selected district. If this is no district selected the enrolment officers list will be filled by all districts' enrolment officers*

    * ``Payer``

      Select the payer from the drop down list by clicking on the right arrow. By selecting any of the options a user can filter the report on a particular payer. This filter is not mandatory; leave it blank to preview the report on all the payers.

    * ``Claim Status``

      Select the claim status from the drop down list by clicking on the right arrow. By selecting any of the options a user can filter the report on a particular claim status. This filter is not mandatory, leave it blank to preview the report on all the claim statuses.

    * ``Sorting``

      Select the way of sorting of records in the report from the list of available ways of sorting **(Renewal Date, Receipt Number, Enrolment Officer)**.

    * ``Previous``

      Select the previous reports from the drop down list by clicking on the right arrow. By selecting any of the options a user can fetch a report which was produced before. *Note: This filter is available only for Matching Funds Report.*

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 223<image223>`) by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

        - At anytime during the use of the pop-up, the user can see the date of **today**.
        - Clicking on *today* will close the pop-up and display the today’s date in the corresponding date entry box.
        - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
        - Clicking on the arrow to the left displays the previous month.
        - Clicking on the arrow on the right will displays the following month.
        - Clicking on the month will display all the months for the year.
        - Clicking on the year will display a year selector.

      .. _image223:
      .. |logo48| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo49| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo50| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +----------++----------++----------+
      | |logo48| || |logo49| || |logo50| |
      +----------++----------++----------+

        `Image 223 - Calendar Selector - Search Panel`

 #. **Report Type Selector**

    This panel contains a list of available report types. A user can select to create a desired report by clicking on the report type list item (:ref:`Image 224<image224>`) and narrow the report using the criteria being shown on the panel above, and then click the preview button to create the report. Available report types are:

      - Primary Operational Indicators Report.
      - Derived Operational Indicators Report.
      - Contribution Collection Report.
      - Product Sales Report.
      - Contribution Distribution.
      - User Activity Report.
      - Enrolment Performance Indicators
      - Status of Registers
      - Insures without Photos.
      - Matching Funds.
      - Claim Overview.
      - Payment Category Overview.
      - Families and Insurees Overview.
      - Pending Insurees.
      - Percentage of Referrals.
      - Capitation Payment

    .. _image224:
    .. figure:: /img/user_manual/image192.png
      :align: center

      `Image 224 - Report Type Selector`

 #. **Button Panel**

    * ``Preview button``

      By clicking on this button, the system will process the selected report type basic on the corresponding criteria submitted and re-direct current user to `Report Page <#reports>`__, for previewing the processed report. At any time the user clicks on the preview button, the current criteria will be saved in the session and can be reused later in the same session and for other report types where the same criteria are found.

    * ``Cancel button``

      By clicking on this button, the current user will be re-directed to the `Home Page <#image-2.2-home-page>`__.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur if there was an error at any time during the processing of the reports.

Report Preview
""""""""""""""

 The report viewer offers the facility to navigate through the report either by using the arrows or by typing in a page number at the top of the report. Another feature of the report viewer is to export the report in different formats. Currently system supports three formats; Word, Excel and PDF. Select the desired format from the list by clicking on the Export link. Use the ``Go Back to Selector`` link to go back to the previous selection page.

 Below are the types of reports as they can be seen in the report page.

 #. **primary operational indicators  - policies report**

    The report provides aggregate data relating to policies and insurees according to insurance products. The report can be run by users with the role Manager. The table below will provide an overview on primary indicators of the report.

    .. list-table:: Table  Overview of Policies indicators
        :widths: 1 2 3 7
        :header-rows: 1
        :stub-columns: 1
        :class: longtable

        * - **Code**
          - **Primary indicators**
          - **Dimension**
          - **Description**

        * - P1
          - Number of policies
          - Time, Insurance product
          - The number of policies of given insurance product on the last day of a respective period (Status of the policy is Active, the last day of period is within <Effective date, Expiry day>)

        * - P2
          - Number of new policies
          - Time, Insurance product
          - The number of new policies of given insurance product during a respective period (Enrolment date is within the respective period, there is ``no`` preceding policy with the same (or before converted) insurance product forgiven policy)

        * - P3
          - Number of suspended policies
          - Time, Insurance product
          - The number of policies for given insurance product that were suspended during a respective period (Status of the policy is Suspended, suspension took place within the respective period)

        * - P4
          - Number of expired policies
          - Time, Insurance product
          - The number of policies for given insurance product that expired during a respective period (Status of the policy is Expired,expiration took place within the respective period)

        * - P5
          - Number of renewals
          - Time, Insurance product
          - The number of policies that were renewed forgiven insurance product (or a converte done) during a respective period ( Enrolment date is within the respective period, there is a preceding policy with the same (or before converted) product forgiven

        * - P6
          - Number of insurees
          - Time, Insurance product
          - The number of insurees covered by policies of given insurance product on the last day of a respective period (An insuree belongs to a family with an active coverage on the last day of the respective period-see P1 )

        * - P7
          - Number of newly insured insurees
          - Time, Insurance product
          - The number of insurees covered by new policies of given insurance product during a respective period (An insuree belongs to a family with newly acquired policy during the respective period-see P2 )

        * - P8
          - Newly collected Contributions
          - Time, Insurance product
          - Amount of acquired Contributions (for policies of given insurance product) during a respective period ( Date of payment of a Contribution is within the respective period)

        * - P9
          - Available Contributions
          - Time, Insurance product
          - Amount of Contributions that should be allocated for policies of given insurance product for a respective period provided a uniform distribution throughout the insurance period takes place. (If the respective period overlaps with <Effective date, Expiry day> of a policy then a proportional part of corresponding Contributions relating to the respective period is included in available Contributions)


    Below is an example of the report:

    .. _image225:
    .. figure:: /img/user_manual/image193.png
      :align: center

      `Image 225 - Preview – Primary Operational Indicators - Policies Report`

 #. **primary operational indicators  - claims report**

    The report provides aggregate data relating to policies and insurees according to insurance products. The report can be run by users with the role Manager. The table below will provide an overview on primary indicators of the report.

    .. list-table:: Table Overview of operational indicators
        :widths: 1 2 3 7
        :header-rows: 1
        :stub-columns: 1
        :class: longtable
  
        * - **Code** 
          - **Primary indicators** 
          - **Dimension** 
          - **Description**

        * - P10 
          - Number of claims 
          - Time, Health facility, Insurance product 
          - The number of claims for given insurance product that emerged during a respective period (Start dateof a claim is within the respective period) 

        * - P11 
          - Amount remunerated
          - Time, Health facility, Insurance product 
          - Amount remuneratedfor claims for given insurance product that emerged during a respective period (Start dateof a claim is within the respective period) 

        * - P12 
          - Number of rejected claims 
          - Time, Health facility, Insurance product 
          - The number of claims for given insurance product that emerged during a respective period and were rejected (Start dateof a claim is within the respective period and the Status approval ofthe claim is Rejected)

    Below is an example of the report:

    .. _image226:
    .. figure:: /img/user_manual/image194.png
      :align: center

      `Image 226 - Preview – Primary Operational Indicators - Claims Report`

 #. **derived operational indicators report**

    The report provides operational indicators derived from primary operational indicators. The report can be run by users with the role Manager. The table below will provide an overview on the actual derived indicators provided by the report.

    .. list-table:: Table Overview of derived operational indicators
        :widths: 1 2 3 7
        :header-rows: 1
        :stub-columns: 1
        :class: longtable

        * - **Code**
          - **Derived**
          - **Dimension**
          - **Description**

        * - D1
          - Incurred claims ratio
          - Time, Insurance product
          - It is the ratio P11/P9

        * - D2
          - Renewal ratio
          - Time, Insurance product
          - It is the ratio P5/P4

        * - D3
          - Growth ratio
          - Time, Insurance product
          - It is the ratio P2/P1-for immediately preceding period

        * - D4
          - Promptness of claims settlement
          - Time, Insurance product
          - It is the average (date of sending to payment- Date of submission of the claim) for all claims relating to given insurance product and emerging in a respective period Date of sending of payment is not in the structure of Claim, it has to be retrieved from a journal-can be?)

        * - D5
          - Claims settlement ratio
          - Time, Health facility, Insurance product
          - It is the ratio (P10-P12)/P10

        * - D6
          - Number of claims per insuree
          - Time, Insurance product
          - It is the ratio P10/P6

        * - D7
          - Average cost per claim
          - Time, Health facility, Insurance product
          - It is the ratio P11/P10

        * - D8
          - Satisfaction level
          - TimeDistrict, Health facility
          - The average mark from feedbacks received in a respective period

        * - D9
          - Feedback response ratio
          - Time, District, Health facility
          - The ratio of number of feedbacks received (up to time of creation of the report) and number of feedbacks asked for in a respective period

    Below is an example of the report:

    .. _image227:
    .. figure:: /img/user_manual/image195.png
      :align: center

      `Image 227 - Preview – Derived Operational Indicators Report`

 #. **Contribution collection report**

    The report lists all actual payments of contributions according to insurance products in the defined period. The report can be used as input to an accounting system. The report can be run by users with the role Accountant. Payments are assigned to the specified period according to the actual date of payment.

    Below is an example of the report:

    .. _image228:
    .. figure:: /img/user_manual/image196.png
      :align: center

      `Image 228 - Preview – Contribution Collection Report`

 #. **product sales report**

    The report provides overview of selling of policies according to insurance products in terms of calculated contributions (not necessarily actually paid). The report can be run by users with the role Accountant. Policies are assigned to the specified period according to their effective days.

    Below is an example of the report:

    .. _image229:
    .. figure:: /img/user_manual/image197.png
      :align: center

      `Image 229 - Preview – Product Sales Report`

 #. **Contribution distribution report**

    The report provides proportional amount of actually paid contributions allocated by openIMIS to specific months according to insurance products. The report can be run by users with the role Accountant. This report shows the information about the **Total collection**, **Allocated amount** and **Not allocated** amount for contributions in the specified period.

    **Allocated** amount is the proportionally calculated amounts of contributions paid covering the month. **Not Allocated** amount is the amount collected for contributions that have a start date in the future (after the month in question).

    Below is an example of the report:

    .. _image230:
    .. figure:: /img/user_manual/image198.png
      :align: center

      `Image 230 - Preview – Contribution Distribution Report`

 #. **user activity report**

    The report shows activities of users according to types of activities and types of entities to which the activities relate. The report can be run by users with the role openIMIS Administrator. Below is an example of the report:

    .. _image231:
    .. figure:: /img/user_manual/image199.png
      :align: center

      `Image 231 - Preview – User Activity Report`

 #. **enrolment performance indicator report**

    The report provides overview of activity of enrolment officers. The report can be run by users with the role Manager. Below is an example of the report:

    .. _image232:
    .. figure:: /img/user_manual/image200.png
      :align: center

      `Image 232 - Preview – Enrolment Performance Indicator Report`

 #. **status of registers report**

    The report provides an overview of the number of items in registers according to districts. The report can be run by users with the role Scheme Administrator. Below is an example of the report:

    .. _image233:
    .. figure:: /img/user_manual/image201.png
      :align: center

      `Image 233 - Preview – Status of Registers Report`

 #. **insurees without photos**

    The report lists all insurees according to enrolment officers that have not assigned a photo. The report can be run by users with the role Accountant. Below is an example of the report:

    .. _image234:
    .. figure:: /img/user_manual/image202.png
      :align: center

      `Image 234 - Preview – Insurees without photos`

 #. **matching funds**

    The report lists all families/groups according to insurance products and (institutional) payers that paid contributions in the specified period. This report is useful for claiming of subsidies for running of health insurance schemes. The report can be run by users with the role Accountant. Below is an example of the report:

    .. _image235:
    .. figure:: /img/user_manual/image203.png
      :align: center

      `Image 235 - Preview –Matching Funds`

 #. **claim overview**

    The report provides detailed data about results of processing of claims in openIMIS according to insurance products and health facilities. The report can be used as a tool for communication between a health insurance scheme and its contractual health facilities. The report can be run by users with the role Accountant. Claims are assigned to the specified period according to date of provision of health care (in case of in-patient care according to the date of discharge). Below is an example of the report:

    .. _image236:
    .. figure:: /img/user_manual/image204.png
      :align: center

      `Image 236 Preview – Claim Overview`

 #. **payment category overview**

    The report provides split of total contributions according to their categories. The report can be run by users with the role Accountant. Contributions are assigned to the specified period according to actual payment date. Below is an example of the report:

    .. _image237:
    .. figure:: /img/user_manual/image205.png
      :align: center

      `Image 237 - Preview – Payment Category Overview`

 #. **Families and Insurees Overview report**

    The report provides an overview of enrolled families/groups and their members in specified location within the specified period. The report can be run by users with the role Accountant. Below is an example of the report:

    .. _image238:
    .. figure:: /img/user_manual/image206.png
      :align: center

      `Image 238 - Preview – Families and Insurees Overview Report`

 #. **Percentage of Referrals report**

    The report lists all primary health care facilities (the category is Dispensary and Health Centre) in the selected district and for each such health facilities provides the following indicators:

      a) The number of visits (claims) of the primary health care facility in the selected period.
      b) The number of out-patient visits that have Visit Type equal to Referral in all other health facilities (irrespective of the district) for insurees with the First Service Point in the respective primary health care facility.
      c) The number of in-patient stays that have Visit Type equal to Referral in all health facilities-hospitals (irrespective of the district) for insurees with the First Service Point in the respective primary health care facility.

    The report can be run by users with the role Accountant. Below is an example of the report:

    .. _image239:
    .. figure:: /img/user_manual/image207.png
      :align: center

      `Image 239 - Preview – Percentage of Referrals Overview Report`

 #. **Pending Insurees report**

    The report lists all insurees whose photos have been sent to openIMIS but who has no record in openIMIS yet. The report can be run by users with the role Accountant.  Below is an example of the report:

    .. _image240:
    .. figure:: /img/user_manual/image208.png
      :align: center

      `Image 240 - Preview – Pending Insurees Report`

 #. **Renewals report**

    The report lists all renewed policies in given period for given insurance product and optionally for given enrolment officer. The families that have at least one payment of contributions in given period of time are included in the report. The report can be run by users with the role Accountant. Below is an example of the report:

    .. _image241:
    .. figure:: /img/user_manual/image209.png
      :align: center

      `Image 241 - Preview – Renewals Report`

 #. **Capitation Payment Report**

    The report lists capitation payments for all health facilities specified in the `capitation formula <#capitation-payment>`__ for specified month and for given insurance product. The report can be run by users with the role Accountant. Below is an example of the report:

    .. _image242:
    .. figure:: /img/user_manual/image210.png
      :align: center

      `Image 242 - Preview –Capitation Payment Report`

Utilities
^^^^^^^^^

  Access to the ``Utilities`` is restricted to the users with the role of openIMIS Administrator.

  The ``Utilities`` is the place for database administration. By having access to this page, it is possible to backup and restore the openIMIS operational database and also to execute SQL Scripts (patches provided for maintenance or update of the database). At the top of the page, the current “Backend” version is displayed for reference.

Navigation
""""""""""

  All functionality for use with the administration of utilities can be found under the main menu ``Tools``, sub menu ``Utilities``

  .. _image243:
  .. figure:: /img/user_manual/image211.png
    :align: center

    `Image 243 - Navigation Utilities`

  Clicking on the sub menu ``Utilities`` re-directs the current user to the `Utilities Page. <#image-6.75-utilities-page>`__

  .. _image244:
  .. figure:: /img/user_manual/image212.png
    :align: center

    `Image 244 - Utilities Page`

Backup
""""""

  Backup utility can be found in the top panel of the `Utilities Page <#Utilities>`_. By default the path of the backup folder will be populated from the default table. User can change the path according to the requirement. Next to the textbox user can see one heck box called ``Save Path``. If user wants to update the backup folder in default table then this check box should be in checked state. Otherwise system will take the backup on the folder assigned by the user but it will not be updated in database. So next time when user comes on the `Utilities Page <#Utilities>`_, the textbox will be populated with the original path. After the path has been entered user can just click on the ``Backup button`` to start the process and a progress bar will be appeared on the screen. Users are requested to be patient while the system performs the task.

  .. _image245:
  .. figure:: /img/user_manual/image213.png
    :align: center

    `Image 245 - Backup is in progress`

Restore
"""""""

  Restore utility can be found in the second panel of the `Utilities Page <#Utilities>`_. User will have to put the path of the backup file to be restored. After the path has been entered user can just click on the ``Restore`` button to start the process and a progress bar will be appeared on the screen. Users are requested to be patient while the system performs the task.

  .. _image246:
  .. figure:: /img/user_manual/image213.png
    :align: center

    `Image 246 - Backup is in progress`

Execute script
""""""""""""""

  Execute script can be found in the third panel of the `Utilities Page <#Utilities>`_. User will have to choose the script by clicking on the browse button. User will have to select the file only with the ".isf" extension. After the file has been chosen, user can just click on the ``Execute`` button to run the script. Users are requested to be patient while the system is executing the script. After the script is executed successfully, backed version will be updated to the latest version. If user will try to run the lower or the equal version's script then system will prompt the user with the appropriate message.

Funding
^^^^^^^

  Access to the ``Funding`` is restricted to the users with the role of Accountant.

  The ``Funding`` is the place where funding from external authorities (payers) can be for entered. openIMIS creates internally one fictive family/group (the insurance number of the head of the fictive family/group is 999999999, the name is *Funding* and the other name is *Funding* as well) for the district for which a funding is done. Each entering of a fund results in creation of a fictive policy for the corresponding fictive family/group with paid contribution in the amount of the funding. The fictive policy is active since the date of payment of the corresponding fund. These fictive policies are overpaid as these funds are usually much higher than the contribution rate for a single family/member of the group but it doesn’t matter. External funding corresponds to payment of contributions for many families/members of the group in some period. openIMIS can regard funds as standard contributions and its standard functionality can be used for handling of funds. One distinctive feature of payment of funds by means of the fictive policies is that the payments of funds don’t appear in the reports on matching funds generated for funding authorities. So, there is no danger that offices of the scheme administration would acquire new funds based on funding already acquired.

Navigation
""""""""""

  The functionality for entering of funds can be found under the main menu ``Tools``, sub menu ``Funding``

  .. _image247:
  .. figure:: /img/user_manual/image214.png
    :align: center

    `Image 247 - Navigation Funding`

  Clicking on the sub menu ``Funding`` re-directs the current user to the `Funding Page. <#image-6.79-funding-page>`__

Funding Page
""""""""""""

 #. **Data Entry**

    .. _image248:
    .. figure:: /img/user_manual/image215.png
      :align: center

      `Image 248 - Funding Page`

    * ``Region``

      Select the region from the list of regions for which the funding is designated by clicking on the arrow on the right of the selector. *Note: The list will only be filled with the regions assigned to the current logged in user.*

    * ``District``

      Select the district from the list of districts for which the funding is designated. by clicking on the arrow on the right of the selector. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user.*

    * ``Product``

      Select an insurance product from the list of insurance products purchased in the selected district (including national insurance products) for which the funding is designated.

    * ``Payer``

      Select from the list of institutional payers the funding authority/agency.

    * ``Payment Date``

      Enter the date of receiving of the funding.

    * ``Contribution Paid``

      Enter the amount of the funding.

    * ``Receipt Number``

        Enter an identification of the document accompanying the funding.

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. A message confirming that the new password has been saved will appear. The user will be re-directed back to the `Home Page <#image-2.2-home-page>`__.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right side of the corresponding field). The user will be re-directed to the `Home Page <#image-2.2-home-page>`__.

 #. **Cancel**

    By clicking on the Cancel button, the user will be re-directed to the `Home Page <#image-2.2-home-page>`__.

Email Settings
^^^^^^^^^^^^^^

  Access to the ``Email Settigns`` is restricted to the users with the role of Accountant.

  The ``Email Settigns`` is the page where the setting of the outbound email server are entered.

Navigation
""""""""""

  The functionality for entering of funds can be found under the main menu ``Tools``, sub menu ``Email Settigns``

    .. _image276:
    .. figure:: /img/user_manual/topmenu_tool_email.png
      :align: center

      `Image 276 - Navigation Email Settings`

  Clicking on the sub menu ``Email Settigns`` re-directs the current user to the `Email settings Page. <#image-277-email-settings-page>`__

Email settings page
"""""""""""""""""""

 #. **Data Entry**

    .. _image277:
    .. figure:: /img/user_manual/email_settings.png
      :align: center

      `Image 277 - Email settings Page`

    * ``Email``

      SMTP Login to be used on the email server in order to send email

    * ``Password``

      SMTP password to be used on the email server in order to send email.

    * ``SMTP Host``

      SMTP email server address or IP

    * ``Port``

      SMTP email server IP port, standard port are

        * 25 when no encryption is used

        * 465 when implicit encryption is used(depreciated)

        * 587 when explicit encryption is used, see ``Enable SSL``

    * ``Enable SSL``

        Check to box if the SMTP mail server require encryption


Offline mode
------------

Introduction
^^^^^^^^^^^^

  IMIS system can be used in offline mode, which makes it possible for usage by health facilities (HF) and scheme administration offices with low/no internet connectivity.

OFFLINE FACILITIES
^^^^^^^^^^^^^^^^^^

  Facilities available while offline and online in IMIS, are similar with some few differences. The following are the feature wise differences found while using openIMIS in offline mode.

 #. **Login**

    If a user who is logging in is having user role HF Administrator or offline Scheme Administrator and if Heath Facility ID/Scheme Office ID is not set yet, just after clicking login button on the login screen/page, the user will be prompted to enter Health Facility/Scheme Office ID (:ref:`Image 251<image251>`), (:ref:`Image 252<image252>`), only once for that very first time of logging in.

    .. _image251:
    .. figure:: /img/user_manual/image218.png
      :align: center

      `Image 251 - Enter HF ID - HF Administrator Login, openIMIS offline`

    .. _image252:
    .. figure:: /img/user_manual/image219.png
      :align: center

      `Image 252 - Enter Scheme Office ID - offline Scheme Administrator Login, openIMIS offline`

 #. **Information bar**

      Throughout the application, an information bar at the bottom of each page will have a different background colour to that of online openIMIS and on the its right end, there will be shown heath facility code and health facility name / Scheme Office ID submitted (:ref:`Image 253<image253>`), (:ref:`Image 254<image254>`).

      .. _image253:
      .. figure:: /img/user_manual/image220.png
        :align: center

        `Image 253 - Information Bar – Scheme Office, openIMIS offline`

      .. _image254:
      .. figure:: /img/user_manual/image221.png
        :align: center

        `Image 254 - Information Bar - Health Facility, openIMIS offline`

 #. **Menu Access**

    For all users with roles other than HF Administrator and Offline Scheme Administrator , will have the menus available to them as per normal roles' rights in online openIMIS version. Menu access in the offline version is different in following scenarios:

    User with roles HF Administrator and Offline Scheme Administrator can access only ``Users``, ``IMIS Extracts`` and ``Utilities`` menus, while all other users with different roles can access menus just as they would do in the online openIMIS version.

    * ``Extracts``

      Extracts Menu leads an offline user to Extracts control panel. Using this panel, an offline user with rights to this panel can import data from online openIMIS to the local offline IMIS, and can also download claims and enrolments prior to upload them to the online IMIS. This panel is divided into five sections (:ref:`Image 255<image255>`), (:ref:`Image 256<image256>`) If an offline user is HF Administrator, section C will contain facility to ``Download Claims``. If an offline user is Offline Scheme Administrator, section C will contain facility to ``Download Enrolments``

      .. _image255:
      .. figure:: /img/user_manual/image222.png
        :align: center

        `Image 255 - Extracts Control Page, HF Administrator, openIMIS offline`

      .. _image256:
      .. figure:: /img/user_manual/image223.png
        :align: center

        `Image 256 - Extracts Control Page, Offline Scheme Administrator, openIMIS offline`

    * ``section a - import extract``

      This section has a facility to enable synchronization of online openIMIS data with that offline openIMIS data. When online data in a zipped file is obtained (downloaded extraction) from online openIMIS to user local computer, user will use this section to put that data into offline IMIS.

      User has to select a file from a local computer by clicking the 'select file' button on the left side of the section, and in the popup window which appears (:ref:`Image 256<image256>`) user can navigate to the required file and select the file.

      .. _image257:
      .. figure:: /img/user_manual/image224.png
        :align: center

        `Image 257 - Select File Popup Window, Import Extracts, openIMIS offline`

      After clicking the upload button on the very end of right hand side in this section, data in the file will be imported to the offline openIMIS and confirmation will be given as popup messages (:ref:`Image 257<image257>`), (:ref:`Image 258<image258>`).

      .. _image258:
      .. figure:: /img/user_manual/image225.png
        :align: center

        `Image 258 - Popup Window, Import Extracts, HF Administrator, openIMIS offline`

      .. _image259:
      .. figure:: /img/user_manual/image226.png
        :align: center

        `Image 259 - Popup Window, Import Extracts, Offline Scheme Administrator, openIMIS offline`

      User cannot import an extract whose sequence number is same as last one imported; if done so, a popup message (:ref:`Image 260<image260>`) will be shown.

      .. _image260:
      .. figure:: /img/user_manual/image227.png
        :align: center

        `Image 260 - Popup Window, Wrong sequence of an extract file, openIMIS offline`

    * ``section b - import photos``

      Just as the section name implies, this is a section with facility to enable a user synchronize insurees’ photos in online IMIS, with insurees’ photos in offline IMIS. When online insurees’ photos in a zipped file is obtained from online openIMIS to user local computer, user will use this section to put those photos into offline IMIS.

      User has to select a file from a local computer by clicking the 'select file' button on the left side of the section, and in the popup window which appears (:ref:`Image 261<image261>`), user can navigate to the required file and select the file.

      .. _image261:
      .. figure:: /img/user_manual/image224.png
        :align: center

        `Image 261 - Select File Popup Window, Import Photos, openIMIS offline`

      After clicking the upload button on the very end of right hand side in this section, data in the file will be imported to the offline openIMIS and confirmation will be given as popup messages (:ref:`Image 261<image261>`).

      .. _image262:
      .. figure:: /img/user_manual/offline_extract_photo_conf.png
        :align: center

        `Image 262 - Popup Window, Import Photos, openIMIS offline`

      If importation of photo is not done due to some reason, the above popup message will not be shown, instead system will issue proper popup message to notify a user what went wrong and what is to be done.

    * ``section c - download claim xmls``

      This section has facility to enable offline HF Administrator download to a zipped file all offline claims. By clicking the download button on the right hand side, the user initiate download process and all offline claims will be downloaded to a default downloads folder in user's local computer or a prompt of 'where to save file' will be displayed by browser'. User can navigate through folder in his/her local computer to find the file downloaded. If no new claims found, a message will be displayed.

    * ``download enrolment xmls``

      This section has facility to enable Offline Scheme Administrator download to a zipped file all offline enrollments of families, insurees, policies and contributions. By clicking the download button on the right hand side, the user initiate download process. If no enrolment found, a popup message box (:ref:`Image 262<image262>`) will appear, notifying the user. Otherwise enrollments will be downloaded in a zipped file and a confirmation popup message (:ref:`Image 264<image264>`) will appear

      .. _image263:
      .. figure:: /img/user_manual/image228.png
        :align: center

        `Image 263 - Popup Window, Download Enrolments, openIMIS offline`

      .. _image264:
      .. figure:: /img/user_manual/image229.png
        :align: center

        `Image 264 - Popup Window, Download Enrolments, openIMIS offline`

    * ``section d - buttons``

      This section has a cancel button, which when clicked will take the current user to the Home page.

    * ``section e - information bar``

      Information bar at the bottom will show different notification messages in blue color depending on the actions of the user. Such actions and messages may be:

      a) No Previous Extract Found

        This message is seen at the first time when using the system and no any extract has been imported into the offline IMIS

        .. _image265:
        .. figure:: /img/user_manual/image230.png
          :align: center

          `Image 265 - openIMIS Extracts, Information Bar, openIMIS offline`

      b) Last Extract Sequence: <Sequence Number>

        This message is seen, after a single / series of extract importation have been made to the offline openIMIS and that much times will be shown as a sequence number at the end of the message. This enables proper tracking of right extracts to import and use.

        .. _image266:
        .. figure:: /img/user_manual/image231.png
          :align: center

          `Image 266 - openIMIS Extracts, Information Bar, openIMIS offline`

      c) No claims Found

        When HF offline openIMIS user is downloading offline claims and no new offline claims is found, this message is displayed.

        .. _image267:
        .. figure:: /img/user_manual/image232.png
          :align: center

          `Image 267 - openIMIS Extracts, Information Bar, openIMIS offline`

 #. **User**

     Users with role HF Administrator, can create only users with roles: **Receptionist, Claim Administrator** and **HF Administrator** (:ref:`Image 268<image268>`). User with role 'offline NSHIP Administrator', can create only user with role: **Clerk** (:ref:`Image 269<image269>`).

      .. _image268:
      .. figure:: /img/user_manual/image233.png
        :align: center

        `Image 268 - Users Page - HF Administrator, openIMIS offline`

      .. _image269:
      .. figure:: /img/user_manual/image234.png
        :align: center

        `Image 269 - Users Page - Offline Scheme Administrator, openIMIS offline`

 #. **data access**

    - Search / Find

        In all pages in ``Insurees`` and ``Policies`` menus with search / find acility, there will be an extra search criteria (:ref:`image 270<image270>`) to enable search for offline data only. This feature is available if a user is in Offline IMIS.

        .. _image270:
        .. figure:: /img/user_manual/image235.png
          :align: center

          `Image 270 - Search Criteria - offline only data, openIMIS offline`

    - Create / Edit

      Only families, insurees, policies and contributions created/edited while offline, will be available for further manipulation. An online data is available for viewing purposes.

      For an offline user with a right to open ``Insurees`` and ``Policies`` menus, he/she can access all data but can manipulate only that data which was created offline. The rest of the data will be available in read-only mode
