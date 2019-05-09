Medical Items Administration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  The register of Medical Items contains all medical items (drugs, prostheses) that can be included in packages of benefits of insurance products within the health insurance scheme and are remunerated by the scheme administration. Administration of the register of medical items is restricted to users with the role of Scheme Administrator

Pre-conditions
""""""""""""""

  A medical item may only be added or thereafter edited or deleted, after the approval of the management of the scheme administration.

Navigation
""""""""""

  All functionality for use with the administration of medical items can be found under the main menu ``Administration``, sub menu ``Medical Items``

  .. _image29:
  .. figure:: /img/user_manual/image30.png
    :align: center

    `Image 29 - Navigation Medical Items`

  Clicking on the sub menu ``Medical Items`` re-directs the current user to the `Medical Items Control Page <#medical-items-control-page>`__\.

  .. _image30:
  .. figure:: /img/user_manual/image31.png
    :align: center

    `Image 30 - Medical Items Control Page`

Medical Items Control Page
""""""""""""""""""""""""""

  The ``Medical Items Control Page`` is the central point for all medical item administration. By having access to this page, it is possible to add, edit, delete and search. The panel is divided into four panels (:ref:`Image 30<image30>`)

 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. In the case of medical items the following search options are available which can be used alone or in combination with each other.

    * ``Code``

      Type in the beginning of; or the full ``Code``; to search for medical items with a ``Code``, which starts with or matches completely, the typed text.

    * ``Name``

      Type in the beginning of; or the full ``Name`` to search for medical items with a ``Name``, which starts with or matches completely, the typed text.

    * ``Type``

      Select the ``Type``; from the list of types (Drugs, Medical Prostheses) by clicking on the arrow on the right of the selector, to select medical items of a specific type.

    * ``Package``

      Type in the beginning of; or the full ``Package``; to search for medical items with a ``Package``, which starts with or matches completely, the typed text.

    * ``Historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records (:ref:`Image 31<image31>`).

      .. _image31:
      .. figure:: /img/user_manual/image32.png
        :align: center

        `Image 31 - Historical records - Result Panel`

    * ``Search button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the Result Panel.

 #. **Result Panel**

    The result panel displays a list of all medical items found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 32<image32>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

    .. _image32:
    .. figure:: /img/user_manual/image33.png
      :align: center

      `Image 32 - Selected record (blue), hovered records (yellow) - Result Panel`

    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:ref:`Image 33<image33>`)

    .. _image33:
    .. figure:: /img/user_manual/image11.png
      :align: center

      `Image 33 - Page selector- Result Panel`

 #. **Button Panel**

    With exception of the ``Cancel`` button, which re-directs to the `Home Page <#image-2.2-home-page>`__, and the ``Add`` button which re-directs to the `Medical Item Page <#medical-item-page>`__, the button panel (the buttons ``Edit`` and ``Delete``) is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a medical item has been added, updated or deleted or if there was an error at any time during the process of these actions.

Medical Item Page
"""""""""""""""""

 #. **Data Entry**

    .. _image34:
    .. figure:: /img/user_manual/image34.png
      :align: center

      `Image 34 - Medical Item Page`

    * ``Code``

      Enter the code for the medical item. Mandatory, 6 characters.

    * ``Name``

      Enter the name of the medical item. Mandatory, 100 characters maximum.

    * ``Type``

      Choose one from the options available, the type of the medical item. Mandatory.

    * ``Package``

      Enter the package (Indication of type and volume of package in a suitable coding system) for the medical item. Mandatory, 255 characters maximum.

    * ``Price``

      Enter the price (a general price that can be overloaded in pricelists). Full general price including potential cost sharing of an insuree) for the medical item. Mandatory.

    * ``Care Type``

      Choose one from the options available, the limitation of provision of the medical item within the specific type of health care (In-patient, Out-patient or Both). Mandatory.

    * ``Frequency``

      Enter the limitation of frequency of provision in a number of days within which a medical item cannot be provided to a patient not more than once. If the frequency is zero, there is no limitation. *Note: By default the frequency is 0.*

    * ``Patient``

        Choose one or a combination of the options available, to specify which patient type the medical item may be provided to. *Note: By default all patients’ options are checked (selected).*

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Medical Items Control Page <#medical-items-control-page>`__, with the newly saved record displayed and selected in the Result Panel. A message confirming that the medical item has been saved will appear on the Information Panel.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right of the corresponding data field).

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Medical Items Control Page. <#medical-items-control-page>`__

Adding a Medical Item
"""""""""""""""""""""

  Click on the ``Add`` button to re-direct to the `Medical Item Page <#medical-item-page>`__\ .

  When the page opens all entry fields are empty. See the `Medical Item Page <#medical-item-page>`__ for information on the data entry and mandatory fields.

Editing a Medical Item
""""""""""""""""""""""

  Click on the ``Edit`` button to re-direct to the `Medical Item Page <#medical-item-page>`__\ .

  The page will open with the current information loaded into the data entry fields. See the `Medical Item Page <#medical-item-page>`__ for information on the data entry and mandatory fields.

Deleting a Medical Item
"""""""""""""""""""""""

  Click on the ``Delete`` button to delete the currently selected record

  Before deleting a confirmation popup (:ref:`Image 35<image35>`) is displayed, which requires the user to confirm if the action should really be carried out?

  .. _image35:
  .. figure:: /img/user_manual/image24.png
    :align: center

    `Image 35 - Delete confirmation- Button Panel`

  When the medical item is deleted, all records retaining to the deleted medical item will still be available by selecting historical records.
