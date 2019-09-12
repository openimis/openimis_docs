.. include:: /_sidebar.rst.inc

IMIS Extracts
^^^^^^^^^^^^^

  Access to the openIMIS Extracts page is restricted to users with the system role of Scheme Administrator (IMIS Central online) or HF Administrator (IMIS offline installations) or with a role including an access to Tools/Extracts. This page will contain all functionality for data synchronization between IMIS Central and IMIS offline installations as well as the generation of extract files for the mobile phones (Android). Depending on the type of installation, the interface will enable and disable certain functions.

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
