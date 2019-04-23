Heath Facility Claims
^^^^^^^^^^^^^^^^^^^^^

  Access to the ``Health Facility Claims Page`` is restricted to users with the role of Claim Administrator.

Pre-conditions
""""""""""""""

Navigation
""""""""""

  All functionality for use with the administration of health facility claims can be found under the main menu ``Claims``, sub menu ``Health Facility Claims``.

  .. _image136:
  .. figure:: /img/user_manual/image110.png
    :align: center

    `Image 136 - Navigation Health Facility Claims`

  Clicking on the sub menu ``Health Facility Claims`` re-directs the current user to the `Claims Control Page <#_Health_Facility_Claims>`__.

Claims Control Page
"""""""""""""""""""

  .. _claims_control_img:
  .. figure:: /img/user_manual/claims_control.png
    :align: center

    `Image - Claims Control Page`

  The Claims Control Page is the central point for all health facility claim administration. By having access to this panel, it is possible to add, edit and search claims. Claims can be edited only in the state **Entered**. The panel is divided into four panels (:ref:`Image 136<image136>`).

 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. In the case of claims the following search options are available which can be used alone or in combination with each other.

    * ``Region``

      Select the ``Region``; where claiming or searched for health facility is located from the list of regions by clicking on the arrow on the right of the selector to select claims from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected*

    * ``District``

      Select the ``district``; where claiming or searched for health facility is located from the list of districts by clicking on the arrow on the right of the selector to select claims from a specific district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected.*

    * ``HF Code``

      Select the ``HF Code`` (Health Facility Code) from the list of codes of health facilities by clicking on the arrow on the right of the selector, to select claims from a specific health facility. *Note: The list will only be filled with the health facilities belonging to the selected district and assigned to the current logged in user.*

    * ``HF Name``

      Type in the beginning of; or the full ``HF Name`` (Health Facility Name) to search for claims belonging to the health facility whose name start with or match completely the typed text.

    * ``Claim Administrator``

      Select the ``Claim Administrator`` from the list of claim administrators by clicking on the arrow on the right of the selector, to select claims submitted by a specific claim administrator. *Note: The list will only be filled with the claim administrators belonging to the health facility selected.*

    * ``Visit Type``

      Select the ``Visit Type`` from the list of visit types (or hospital stays) by clicking on the arrow on the right of the selector, to select claims with specified visit type.

    * ``Insurance Number``

      Type in the beginning of; or the full ``Insurance Number``, to search for claims, on behalf of insurees with the insurance number which starts with or match completely the typed text.

    * ``Claim No.``

      Type in the beginning of; or the full ``Claim No.``, to search for claims with the specific claim identification which starts with or match completely the typed text.

    * ``Review Status``

      Select the ``Review Status`` from the list of options for review status by clicking on the arrow on the right of the selector, to select claims with specific review status.

    * ``Feedback Status``

      Select the ``Feedback Status`` from the list of options for feedback status by clicking on the arrow on the right of the selector, to select claims with specific feedback status.

    * ``Claim Status``

      Select the ``Claim Status`` from the list of options for claim status by clicking on the arrow on the right of the selector, to select claims with specific claim status.

    * ``Main Dg.``

      Select the ``Main Dg.`` from the list of diagnoses status by by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box, to select claims with main diagnosis.

    * ``Batch Run``

      Select the ``batch run`` from the list of batch runs by clicking on the arrow on the right of the selector, to select claims from specific batch run

    * ``Visit Date From``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Visit Date From`` date which is on or is greater than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.* ``Visit Date From`` should be the day of admission for in-patient care or the visit date in case of out-patient care.

    * ``Visit Date To``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Visit Date From`` date which is on or is less than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.* ``Visit Date To`` should be the day of discharge for in-patient care or the visit date in case of out-patient care.

    * ``Claim Date From``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Claim Date`` date which is on or is greater than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Claim Date To``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Claim Date`` date which is on or is less than the date typed/selected. Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 138<image138>`); by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

        - At anytime during the use of the pop-up, the user can see the date of **today**.
        - Clicking on today will close the pop-up and display the today’s date in the corresponding date entry box.
        - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
        - Clicking on the arrow to the left displays the previous month.
        - Clicking on the arrow on the right will displays the following month.
        - Clicking on the month will display all the months for the year.
        - Clicking on the year will display a year selector.

      .. _image138:
      .. |logo36| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo37| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo38| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +----------++----------++----------+
      | |logo36| || |logo37| || |logo38| |
      +----------++----------++----------+

        `Image 138 - Calendar Selector - Search Panel`

    * ``Search Button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the Result Panel.

 #. **Result Panel**

    The Result Panel displays a list of all claims found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 139<image139>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

    .. _image139:
    .. figure:: /img/user_manual/image112.png
      :align: center

      `Image 139 - Selected record (blue), hovered records (yellow) - Result Panel`

    A maximum of 2000 records can be displayed at one time, in a scroll panel. Further records can be viewed by processing the current loaded claims and search claims again.

 #. **Button Panel**

    With exception of the ``Cancel`` button, which re-directs to the `Home Page <#image-2.2-home-page>`__, and the ``Add`` button which re-directs to the `Claim Page, <#claim-page>`__ the button panel (the buttons Load and Submit) is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

    * ``add``

      By clicking on the add button, the user is directed to the `Claim Page, <#claim-page>`__ where new entries for new claim can be added. When the page opens all entry fields are empty. See the `Claim Page <#claim-page>`__ for information on the data entry and mandatory fields.

    * ``load``

      By clicking on the load button, the user is directed to the `Claim Page <#claim-page>`__, where the current selected claim can be edited (provided it in the state **Entered**).


      The page will open with the current information loaded into the data entry fields. See the `Claim Page <#claim-page>`__ for information on the data entry and mandatory fields.

    * ``submit``

      By clicking on the submit button, claim status of all claims with claim status **Entered** and which have been selected to be submitted by checking the check box on right end of each record, will be submitted.


      On the top of result panel, there is a checkbox to be used to select all claims currently loaded in the result panel and whose claim status is **Entered**, prior to be submitted.


      Once the process is done, a popup window (:ref:`Image 140<image140>`) with the result of the process will be shown.

      .. _image140:
      .. figure:: /img/user_manual/image113.png
        :align: center

        `Image 140 - Submit Claims Prompt – Claims Control Page`

      .. _image141:
      .. figure:: /img/user_manual/image114.png
        :align: center

        `Image 141 - Submitted Claims details – Claims Control Page`

    * ``delete``

      By clicking on the delete button, the current selected claim will be deleted.


      Before deleting a confirmation popup (:ref:`Image 142<image142>`) is displayed, which requires the user to confirm if the action should really be carried out?

      .. _image142:
      .. figure:: /img/user_manual/image115.png
        :align: center

        `Image 142 - Delete confirmation – Claims Control Page`

    * ``cancel``

      By clicking on the ``Cancel`` button, the user will be re-directed to the `Home Page <#image-2.2-home-page>`__.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a claim has been added, updated or deleted or if there was an error at any time during the process of these actions.

Claim Page
""""""""""

 #. **Data Entry**

    .. _claim_add_img:
    .. figure:: /img/user_manual/claim_add.png
      :align: center

      `Image - Claim Page`


    * ``HF Code``

      Displays the code of the health facility. The field is read only (taken over from the `Claims Control Page) <#_Health_Facility_Claims>`__ and cannot be edited.

    * ``HF Name``

      Displays the name of the health facility. The field is read only (taken over from the `Claims Control Page <#_Health_Facility_Claims>`__) and cannot be edited.

    * ``Insurance Number``

      Enter the insurance number of the patient. When done entering this field, the corresponding name of the patient will be filled on the name of the patient (the text box which is read only field and is on the right side of the Insurance Number text field). Mandatory.

    * ``Claim No.``

      Enter the identification of the claim. Mandatory, up to 8 characters. It should be unique within the claiming health facility.

    * ``Main Dg.``

      Select the code of the main diagnosis from the drop down list of diagnosis codes. Mandatory.

    * ``Sec Dg 1``

      Select the code of the first secondary diagnosis from the drop down list of diagnosis codes.

    * ``Sec Dg 2``

      Select the code of the second secondary diagnosis from the drop down  list of diagnosis codes.

    * ``Sec Dg 3``

      Select the code of the third secondary diagnosis from the drop down list of diagnosis codes.

    * ``Sec Dg 4``

      Select the code of the fourth secondary diagnosis from the drop down list of diagnosis codes.

    * ``Claim Administrator``

      Displays code of the claim administrator. The field is read only (taken over from `the Claim Control Page <#_Health_Facility_Claims>`__) and cannot be edited.

    * ``Visit Date From``

      Enter the visit date for out-patient care or the admission date for in-patient care. Mandatory.

    * ``Visit Date To``

      Enter the discharge date for in-patient care.

    * ``Date Claimed``

      Enter the date when the claim was prepared by the health facility.

    * ``Guarantee No.``

      Enter identification of a guarantee letter for prior approval of provision of claimed health care.

    * ``Visit Type``

      Select the type of visit/hospital admission from the drop down list (**Emergency, Referral, Other**)

    * ``Services``

      1. ``service code``

        When entering the service code, a dropdown suggestion box for the available services with the service code or service name matching your typed text will be shown. Available medical services in the dropdown suggestion box are taken over from the pricelist of medical services associated with the claiming health facility. The desired service can then be selected from the dropdown suggestion box by clicking on it using mouse or selecting it using up and down arrows, then pressing Enter key fill the service code text field, together with quantity and value field in the same row.


        Once the selected service has been written on the service data grid row, the dropdown suggestion box will close itself. When needed, the dropdown suggestion box can be closed by clicking any place on the page but outside the dropdown suggestion box.

        .. _image144:
        .. figure:: /img/user_manual/image117.png
          :align: center

          `Image 144 - Services dropdown suggestion box – Claim Page`

      2. ``quantity``

        This field can be filled manually by entering a number in it or automatically is filled by 1 when the service code above is filled, through dropdown suggestion box. It is this field that receives focus after service code is filled above from the dropdown suggestion box.

      3. ``price``

        This field can be filled manually by entering a number in it or automatically is filled when the service code above is filled, through dropdown suggestion box. Automatically filled prices are taken over from the pricelist of medical services associated with the claiming health facility.

      4. ``explanation``

        Enter extra information about the service for the scheme administration (a medical officer of the scheme administrator).

    * ``Items``

      1. ``item code``

        When entering the item code, a dropdown suggestion box for the available items with the item code or item name matching your typed text will be shown. Available medical items in the dropdown suggestion box are taken over from the pricelist of medical items associated with the claiming health facility. The desired item can then be selected from the dropdown suggestion box by clicking on it using mouse or selecting it using up and down arrows, then pressing Enter key to fill the item code text field, together with quantity and value field in the same row.


        Once the selected item has been written on the item data grid row, the dropdown suggestion box will close itself. When needed, the dropdown suggestion box can be closed by clicking any place on the page but outside the dropdown suggestion box.

        .. _image145:
        .. figure:: /img/user_manual/image118.png
          :align: center

          `Image 145 - Items dropdown suggestion box – Claim Page`

      2. ``quantity``

        This field can be filled manually by entering a number in it or automatically is filled by 1 when the item code above is filled, through dropdown suggestion box. It is this filled that receives focus after item code is filled above from the dropdown suggestion box.

      3. ``price``

        This field can be filled manually by entering a number in it or automatically is filled when the item code above is filled, through dropdown suggestion box. Automatically filled prices are taken over from the pricelist of medical items associated with the claiming health facility.

      4. ``explanation``

        Enter extra information about the medical item for the scheme administration (a medical officer of the scheme administrator).

    * ``claimed``

      This field is filled automatically with a new total of quantities multiplied to their corresponding values in both data input grids at any time when there is a change in values in the either quantity fields or value fields anywhere in both data input grids.

    * ``explanation``

      Enter extra information about the whole claim for the scheme administration (medical officer).

    **#  User Controls**

    On top of services input grid panel and items input grid panel, there is a textbox field (:ref:`Image 146<image146>`) and (:ref:`Image 147<image147>`) which is filled with a constant representing the current number of rows in the input grid a user is working with. A user can change the current number of rows in the corresponding data input grid by entered a number of rows greater than existing one. This change is only allowed before a user has made changes to the corresponding data input grid.

    .. _image146:
    .. figure:: /img/user_manual/image119.png
      :align: center

      `Image 146 - Services input grid row number change, input field – Claim Page`

    .. _image147:
    .. figure:: /img/user_manual/image120.png
      :align: center

      `Image 147 - Items input grid row number change, input field – Claim Page`

    A user can manually clear the inputs in the row by clicking the ``Red Cross`` button on the end right of a desired row (:ref:`Image 148<image148>`). This action will require a user to confirm for the clearing process to proceed by choosing either yes / no from the popup window (:ref:`Image 149<image149>`) asking for user confirmation.

    .. _image148:
    .. figure:: /img/user_manual/image121.png
      :align: center

      `Image 148 - Clear row inputs button-Claim Page`

    .. _image149:
    .. figure:: /img/user_manual/image122.png
      :align: center

      `Image 149 - Clearing of a row confirmation – Claim Page`

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the claim. The user stay in the `Claim Page <#claim-page>`__; a message confirming that the claim has been saved will appear on the bottom of the `Claim Page <#claim-page>`__.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk).

 #. **Printing of a claim**

    By clicking on the ``Print`` button, the user will be shown a printable version of the claim details page. The printable version of the claim is available in the following formats (Word, PDF, Excel)

 #. **Creating of a new claim**

    By clicking on the ``Add`` button, the `Claim Page <#claim-page>`__ is cleared (with exception of HF Code, HF Name and Claim Administrator) and it ready for entering of a new claim for the same health facility and of the same claim administrator as before.

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Claims Control Page <#_Health_Facility_Claims>`__\ .
