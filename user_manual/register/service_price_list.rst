.. include:: /_sidebar.rst.inc

Medical Service Price Lists Administration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  Price lists of medical services are tools for specification which medical services and at which prices can be invoiced by contractual health facilities to the scheme administration. Administration of price lists of medical services is restricted to users with the system role of Scheme Administrator or with a role including an access to Administration/Pricelists-Medical Services.

Pre-conditions
""""""""""""""

  A price list of medical services may only be added, after an agreement with a health facility or a group of health facilities on specific prices. Editing of the price list may occur only after an approval of the management of the scheme administration. Deletion of a price list of medical services normally will occur when a price list becomes obsolete.

Navigation
""""""""""

  All functionality for use with the administration of price lists medical services can be found under the main menu ``Administration``, sub menu ``Price Lists`` and sub menu ``Medical Services``

  .. _image36:
  .. figure:: /img/user_manual/image35.png
    :align: center

    `Image 36 - Navigation Medical Services Price Lists`

  Clicking on the sub menu ``Medical Services`` re-directs the current user to the `Price List Medical Services Control Panel. <#price-list-medical-services-control-page>`__

  .. _image37:
  .. figure:: /img/user_manual/image36.png
    :align: center

    `Image 37 - Price List Medical Service Control Panel`

Price List Medical Services Control Page
""""""""""""""""""""""""""""""""""""""""

  The ``Price List Medical Services Control Page`` is the central point for administration of all price lists of medical service. By having access to this panel, it is possible to add, edit, delete and search. The panel is divided into four panels (:ref:`Image 36<image36>`)

 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. In the case of price lists for medical services the following search options are available which can be used alone or in combination with each other.

    * ``Name``

      Type in the beginning of; or the full ``Name``; to search for price lists medical services with a ``Name``, which starts with or matches completely, the typed text.

    * ``Date``

      Type in the full ``Date`` to search for price lists of medical services with a creation ``Date`` which matches completely, the typed date. *Note: You can also use the button next to the date field to select a date.*

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 38<image38>`); by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

      - Anytime during the use of the pop-up, the user can see the date of today.
      - Clicking on today will close the pop-up and display the today’s date in the corresponding date entry box.
      - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
      - Clicking on the arrow to the left displays the previous month.
      - Clicking on the arrow on the right will displays the following month.
      - Clicking on the month will display all the months for the year.
      - Clicking on the year will display a year selector.

      .. _image38:
      .. |logo12| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo13| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo14| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +----------++---------++---------+
      | |logo12| || |logo13||| |logo14||
      +----------++---------++---------+

        `Image 38 - Calendar Selector - Search Panel`

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select price lists of medical services from a specific region. The option **National** means that the price list is common for all regions. *Note: The list will only be filled with the regions assigned to the current logged in user and with the option National. All nationwide pricelists and all regional pricelists relating to the selected region will be found. If no district is selected then also all district pricelists for districts belonging to the selected region and assigned to the currently logged in user will be found.*

    * ``District``

      Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to select price lists of medical services from a specific district. *Note: The list will be only filled with the districts belonging to the selected region. All nationwide pricelists, all regional pricelists relating to the selected region and all district pricelists for the selected district will be found.*

    * ``Historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records (:ref:`Image 39<image39>`)

      .. _image39:
      .. figure:: /img/user_manual/image37.png
        :align: center

        `Image 39 - Historical records - Result Panel`

    * ``Search button``

      Once the criteria have been entered, use the search button to filter  the records, the results will appear in the Result Panel.

 #. **Result Panel**

    The Result Panel displays a list of all price lists of medical services found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 40<image40>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

      .. _image40:
      .. figure:: /img/user_manual/image38.png
        :align: center

        `Image 40 - Selected record (blue), hovered records (yellow) - Result Panel`

    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:ref:`Image 41<image41>`)

    .. _image41:
    .. figure:: /img/user_manual/image11.png
      :align: center

      `Image 41 - Page selector- Result Panel`

 #. **Button Panel**

    With exception of the ``Cancel`` button, which re-directs to the `Home Page <#image-2.2-home-page>`__, and the ``Add`` button which re-directs to the `Price List Medical Service Page <#price-list-medical-services-page>`__, the Button Panel (the buttons ``Edit`` and ``Duplicate`` ) is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a price list of medical services has been added, updated or deleted or if there was an error at any time during the process of these actions.

Price List Medical Services Page
""""""""""""""""""""""""""""""""

 #. **Data Entry**

      .. _image42:
      .. figure:: /img/user_manual/image39.png
        :align: center

        `Image 42 - Price List Medical Service Page`

    * ``Name``

      Enter the name for the price list of medical services. Mandatory, 100 characters maximum.

    * ``Date``

      Enter the creation date for the price list of medical services. *Note: You can also use the button next to the date field to select a date to be entered.*

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to enter the region in which the price list of medical services is to be used. The region **National** means that the price list is common for all regions. *The list will only be filled with the regions assigned to the current logged in user and with the option National.* Mandatory.

    * ``District``

      Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to enter the district in which the price list of medical services is to be used. *Note: The list will be only filled with the districts belonging to the selected region and currently logged in user.* It is not mandatory to enter a district, not selecting a district will mean the price list of medical services is used in all districts of the region or nationwide if the region National is selected.

    * ``Medical Services``

        Select from the list of available medical services the medical services which the price list of medical service should contain, by either clicking on the ``check all`` box at the top of the list of medical services, or by selectively clicking on the ``check box`` to the left of a medical service. The list shows the medical services displaying the code, name, type and price for reference. There is also an extra column, Overrule, which can be used to overrule the pre-set price. By clicking once on the row desired item in the overrule column, a new price can be entered for the individual service. This occurs when price agreed between a health facility or group of health facilities and the health insurance administration differs from the common price in the register of medical services.

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Price List Medical Services Control Page <#price-list-medical-services-control-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the price list medical service has been saved will appear on the Information Panel.

 #. **Mandatory Data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right of the corresponding data field).

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Price List Medical Services Control Page <#price-list-medical-services-control-page>`__\.

Adding a Price List of Medical Services
"""""""""""""""""""""""""""""""""""""""

  Click on the ``Add`` button to re-direct to the `Price List Medical Services Page <#price-list-medical-services-page>`__\.

  When the page opens all entry fields are empty. See the `Price List Medical Services Page <#price-list-medical-services-page>`__ for information on the data entry and mandatory fields.

Editing a Price List of Medical Services
""""""""""""""""""""""""""""""""""""""""

  Click on the ``Edit`` button to re-direct to the `Price List Medical Services Page <#price-list-medical-services-page>`__\.

  The page will open with the current information loaded into the data entry fields. See the `Price List Medical Services Page <#price-list-medical-services-page>`__ for information on the data entry and mandatory fields.

Duplicating a Price List of Medical Services
""""""""""""""""""""""""""""""""""""""""""""

  Click on the ``Duplicate`` button to re-direct to the `Price List Medical Services Page <#price-list-medical-services-page>`__\.

  The page will open with all the current information for the selected pricelist, (except for the pricelist name which should be unique), loaded into the data entry fields. See the `Price List Medical Services Page <#price-list-medical-services-page>`__ for information on the data entry and mandatory fields. To save the record, enter a unique code before clicking on save.

Deleting a Price List of Medical Services
"""""""""""""""""""""""""""""""""""""""""

  Click on the ``Delete`` button to delete the currently selected record.

  Before deleting a confirmation popup (:ref:`Image 43<image43>`) is displayed, which requires the user to confirm if the action should really be carried out?

  .. _image43:
  .. figure:: /img/user_manual/image24.png
    :align: center

    `Image 43 - Delete Confirmation - Button Panel`

  When a price list medical service is deleted, all records retaining to the deleted price list medical service will still be available by selecting historical records.
