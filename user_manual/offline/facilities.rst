

Offline Facilities
^^^^^^^^^^^^^^^^^^

  Facilities available while offline and online in IMIS, are similar with some few differences. The following are the feature wise differences found while using openIMIS in offline mode.

 #. **Login**

    If a user who is logging in is having user role HF Administrator or offline Scheme Administrator and if Heath Facility ID/Scheme Office ID is not set yet, just after clicking login button on the login screen/page, the user will be prompted to enter Health Facility/Scheme Office ID (:numref:`image251`), (:numref:`image252`), only once for that very first time of logging in.

    .. _image251:
    .. figure:: /img/user_manual/image218.png
      :align: center

      `Enter HF ID - HF Administrator Login, openIMIS offline`

    .. _image252:
    .. figure:: /img/user_manual/image219.png
      :align: center

      `Enter Scheme Office ID - offline Scheme Administrator Login, openIMIS offline`

 #. **Information bar**

      Throughout the application, an information bar at the bottom of each page will have a different background colour to that of online openIMIS and on the its right end, there will be shown heath facility code and health facility name / Scheme Office ID submitted (:numref:`image253`), (:numref:`image254`).

      .. _image253:
      .. figure:: /img/user_manual/image220.png
        :align: center

        `Information Bar – Scheme Office, openIMIS offline`

      .. _image254:
      .. figure:: /img/user_manual/image221.png
        :align: center

        `Information Bar - Health Facility, openIMIS offline`

 #. **Menu Access**

    For all users with roles other than HF Administrator and Offline Scheme Administrator , will have the menus available to them as per normal roles' rights in online openIMIS version. Menu access in the offline version is different in following scenarios:

    User with roles HF Administrator and Offline Scheme Administrator can access only ``Users``, ``IMIS Extracts`` and ``Utilities`` menus, while all other users with different roles can access menus just as they would do in the online openIMIS version.

    * ``Extracts``

      Extracts Menu leads an offline user to Extracts control panel. Using this panel, an offline user with rights to this panel can import data from online openIMIS to the local offline IMIS, and can also download claims and enrolments prior to upload them to the online IMIS. This panel is divided into five sections (:numref:`image255`), (:numref:`image256`) If an offline user is HF Administrator, section C will contain facility to ``Download Claims``. If an offline user is Offline Scheme Administrator, section C will contain facility to ``Download Enrolments``

      .. _image255:
      .. figure:: /img/user_manual/image222.png
        :align: center

        `Extracts Control Page, HF Administrator, openIMIS offline`

      .. _image256:
      .. figure:: /img/user_manual/image223.png
        :align: center

        `Extracts Control Page, Offline Scheme Administrator, openIMIS offline`

    * ``section a - import extract``

      This section has a facility to enable synchronization of online openIMIS data with that offline openIMIS data. When online data in a zipped file is obtained (downloaded extraction) from online openIMIS to user local computer, user will use this section to put that data into offline IMIS.

      User has to select a file from a local computer by clicking the 'select file' button on the left side of the section, and in the popup window which appears (:numref:`image256`) user can navigate to the required file and select the file.

      .. _image257:
      .. figure:: /img/user_manual/image224.png
        :align: center

        `Select File Popup Window, Import Extracts, openIMIS offline`

      After clicking the upload button on the very end of right hand side in this section, data in the file will be imported to the offline openIMIS and confirmation will be given as popup messages (:numref:`image257`), (:numref:`image258`).

      .. _image258:
      .. figure:: /img/user_manual/image225.png
        :align: center

        `Popup Window, Import Extracts, HF Administrator, openIMIS offline`

      .. _image259:
      .. figure:: /img/user_manual/image226.png
        :align: center

        `Popup Window, Import Extracts, Offline Scheme Administrator, openIMIS offline`

      User cannot import an extract whose sequence number is same as last one imported; if done so, a popup message (:numref:`image260`) will be shown.

      .. _image260:
      .. figure:: /img/user_manual/image227.png
        :align: center

        `Popup Window, Wrong sequence of an extract file, openIMIS offline`

    * ``section b - import photos``

      Just as the section name implies, this is a section with facility to enable a user synchronize insurees’ photos in online IMIS, with insurees’ photos in offline IMIS. When online insurees’ photos in a zipped file is obtained from online openIMIS to user local computer, user will use this section to put those photos into offline IMIS.

      User has to select a file from a local computer by clicking the 'select file' button on the left side of the section, and in the popup window which appears (:numref:`image261`), user can navigate to the required file and select the file.

      .. _image261:
      .. figure:: /img/user_manual/image224.png
        :align: center

        `Select File Popup Window, Import Photos, openIMIS offline`

      After clicking the upload button on the very end of right hand side in this section, data in the file will be imported to the offline openIMIS and confirmation will be given as popup messages (:numref:`image261`).

      .. _image262:
      .. figure:: /img/user_manual/offline_extract_photo_conf.png
        :align: center

        `Popup Window, Import Photos, openIMIS offline`

      If importation of photo is not done due to some reason, the above popup message will not be shown, instead system will issue proper popup message to notify a user what went wrong and what is to be done.

    * ``section c - download claim xmls``

      This section has facility to enable offline HF Administrator download to a zipped file all offline claims. By clicking the download button on the right hand side, the user initiate download process and all offline claims will be downloaded to a default downloads folder in user's local computer or a prompt of 'where to save file' will be displayed by browser'. User can navigate through folder in his/her local computer to find the file downloaded. If no new claims found, a message will be displayed.

    * ``download enrolment xmls``

      This section has facility to enable Offline Scheme Administrator download to a zipped file all offline enrollments of families, insurees, policies and contributions. By clicking the download button on the right hand side, the user initiate download process. If no enrolment found, a popup message box (:numref:`image262`) will appear, notifying the user. Otherwise enrollments will be downloaded in a zipped file and a confirmation popup message (:numref:`image264`) will appear

      .. _image263:
      .. figure:: /img/user_manual/image228.png
        :align: center

        `Popup Window, Download Enrolments, openIMIS offline`

      .. _image264:
      .. figure:: /img/user_manual/image229.png
        :align: center

        `Popup Window, Download Enrolments, openIMIS offline`

    * ``section d - buttons``

      This section has a cancel button, which when clicked will take the current user to the Home page.

    * ``section e - information bar``

      Information bar at the bottom will show different notification messages in blue color depending on the actions of the user. Such actions and messages may be:

      a) No Previous Extract Found

        This message is seen at the first time when using the system and no any extract has been imported into the offline IMIS

        .. _image265:
        .. figure:: /img/user_manual/image230.png
          :align: center

          `openIMIS Extracts, Information Bar, openIMIS offline`

      b) Last Extract Sequence: <Sequence Number>

        This message is seen, after a single / series of extract importation have been made to the offline openIMIS and that much times will be shown as a sequence number at the end of the message. This enables proper tracking of right extracts to import and use.

        .. _image266:
        .. figure:: /img/user_manual/image231.png
          :align: center

          `openIMIS Extracts, Information Bar, openIMIS offline`

      c) No claims Found

        When HF offline openIMIS user is downloading offline claims and no new offline claims is found, this message is displayed.

        .. _image267:
        .. figure:: /img/user_manual/image232.png
          :align: center

          `openIMIS Extracts, Information Bar, openIMIS offline`

 #. **User**

     Users with role HF Administrator, can create only users with roles: **Receptionist, Claim Administrator** and **HF Administrator** (:numref:`image268`). User with role 'offline NSHIP Administrator', can create only user with role: **Clerk** (:numref:`image269`).

      .. _image268:
      .. figure:: /img/user_manual/image233.png
        :align: center

        `Users Page - HF Administrator, openIMIS offline`

      .. _image269:
      .. figure:: /img/user_manual/image234.png
        :align: center

        `Users Page - Offline Scheme Administrator, openIMIS offline`

 #. **data access**

    - Search / Find

        In all pages in ``Insurees`` and ``Policies`` menus with search / find acility, there will be an extra search criteria (:numref:`image270`) to enable search for offline data only. This feature is available if a user is in Offline IMIS.

        .. _image270:
        .. figure:: /img/user_manual/image235.png
          :align: center

          `Search Criteria - offline only data, openIMIS offline`

    - Create / Edit

      Only families, insurees, policies and contributions created/edited while offline, will be available for further manipulation. An online data is available for viewing purposes.

      For an offline user with a right to open ``Insurees`` and ``Policies`` menus, he/she can access all data but can manipulate only that data which was created offline. The rest of the data will be available in read-only mode
