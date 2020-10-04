

Heath Facility Claims
^^^^^^^^^^^^^^^^^^^^^

  Access to the ``Health Facility Claims Page`` is restricted to users with the role of Claim Administrator.

Pre-conditions
""""""""""""""

Navigation
""""""""""

  All functionality for use with the administration of health facility claims can be found under the main menu ``Claims``, sub menu ``Health Facility Claims``.

  .. _image136:
  .. figure:: /img/user_manual/claim.menu_hf.png
    :align: center

    `Image - Navigation Health Facility Claims`

  Clicking on the sub menu ``Health Facility Claims`` re-directs the current user to the :ref:`Claims Control Page  <health_facility_claims>`.

.. _health_facility_claims:

Claims Control Page
"""""""""""""""""""

  .. _claims_control_img:
  .. figure:: /img/user_manual/claim.control_page.png
    :align: center

    `Image - Claims Control Page`

  The Claims Control Page is the central point for all health facility claim administration. By having access to this panel, it is possible to add, edit and search claims. Claims can be edited only in the state **Entered**. The panel is divided into four panels (:numref:`claims_control_img`).

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

      Select the ``Main Dg.`` from the list of diagnoses status by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box, to select claims with main diagnosis.

    * ``Batch Run``

      Select the ``batch run`` from the list of batch runs by clicking on the arrow on the right of the selector, to select claims from specific batch run

    * ``Visit Date From``

      Type in a date; or use the Date Selector (:numref:`cal_picker_hfc`), to search for claims with a ``Visit Date From`` date which is on or is greater than the date typed/selected. *Note. To clear the date entry box; use the ``Clear`` button on the date picker popup*. ``Visit Date From`` should be the day of admission for in-patient care or the visit date in case of out-patient care.

    * ``Visit Date To``

      Type in a date; or use the Date Selector (:numref:`cal_picker_hfc`), to search for claims with a ``Visit Date From`` date which is on or is less than the date typed/selected. *Note. To clear the date entry box; use the ``Clear`` button on the date picker popup*. ``Visit Date To`` should be the day of discharge for in-patient care or the visit date in case of out-patient care.

    * ``Claim Date From``

      Type in a date; or use the Date Selector (:numref:`cal_picker_hfc`), to search for claims with a ``Claim Date`` date which is on or is greater than the date typed/selected. *Note. To clear the date entry box; use the ``Clear`` button on the date picker popup**

    * ``Claim Date To``

      Type in a date; or use the Date Selector (:numref:`cal_picker_hfc`), to search for claims with a ``Claim Date`` date which is on or is less than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key*.



      .. _cal_picker_hfc:
      .. list-table:: Date Picker
        :widths: 1 1 1

        * - .. figure:: /img/user_manual/date_picker.day.png
              :align: center

              `Day picker`
          - .. figure:: /img/user_manual/date_picker.month.png
              :align: center

              `Month picker`
          - .. figure:: /img/user_manual/date_picker.year.png
              :align: center

              `Year picker`
        * - At anytime during the use of the pop-up, the user can see the date of **today**.
            Clicking on a day will close the pop-up and display the date

          - Clicking on the arrow to the left displays the previous month.
            Clicking on the arrow on the right will displays the following month.

          - Clicking on the year will display a year selector.


    * ``Search Button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the Result Panel.

 #. **Result Panel**

    The Result Panel displays a list of all claims found, matching the selected criteria in the search panel. The currently selected record is highlighted with light grey. (:numref:`image139`). Double click on the line re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

    .. _image139:
    .. figure:: /img/user_manual/claim.search_result.png
      :align: center

      `Selected record (grey) - Result Panel`

    A maximum of 10 records can be displayed per default but it can be changed by configuration (`gitHub <https://github.com/openimis/openimis-fe-claim_js>`_), in a scroll panel. Further records can be viewed by either changing the page or deleting/submitting the current loaded claims and search claims again.

 #. **Actions**

    Modular openIMIS comes with `Material UI <https://material-ui.com/>`_ this means that there is a single button (:numref:`actions_btn`) which fonction will change depending on the context (Icon change), for less used functions a tree dots menu is available (:numref:`image_3d_claim_hf`) only when claim(s) are selected. By double-clicking on the claim line, the user is directed to the :ref:`Claim Page  <claim-page>`, where the current selected claim can be edited (provided it in the state **Entered**), this page will open with the current information loaded into the data entry fields. See the :ref:`Claim Page  <claim-page>` for information on the data entry and mandatory fields.


    .. _actions_btn:
    .. list-table:: Materal icons

      * - .. _mat_add:
          .. figure:: /img/user_manual/mat.add.png
            :align: center

            `Add`
        - .. _mat_save:
          .. figure:: /img/user_manual/mat.save.png
            :align: center

            `Save`

        - .. _mat_back:
          .. figure:: /img/user_manual/mat.back.png
            :align: center

            `Back`
        - .. _mat_print:
          .. figure:: /img/user_manual/mat.print.png

            `Print`

    .. _image_3d_claim_hf:
    .. list-table:: claims actions

      * - .. _mat_select_all:
          .. figure:: /img/user_manual/mat.select_all.png
            :align: center

            `select all`
        - .. _mat_3d:
          .. figure:: /img/user_manual/mat.3d.png
            :align: center

            `tree dots`
        - .. _mat_hf_claim_menu:
          .. figure:: /img/user_manual/claim.hf_3d.png
            :align: center

            `tree dots menu`


    * ``add``

      By clicking on the add button (:numref:`mat_add`), the user is directed to the `Claim Page, <#claim-page>`__ where new entries for new claim can be added. When the page opens all entry fields are empty. See the :ref:`Claim Page  <claim-page>` for information on the data entry and mandatory fields.


    * ``Submit selected``

      By clicking on the submit selected manu (:numref:`mat_hf_claim_menu`), claim status of all selected claims with the status **Entered** will be submitted.

      Once the process is done, a popup window ( :numref:`image141` ) with the result of the process will be shown.

      .. _image141:
      .. figure:: /img/user_manual/claim.submit_details.png
        :align: center

        `Submitted Claims details – Claims Control Page`

    * ``delete selected``

      By clicking on the delete selected menu, the current selected claim will be deleted.


      Before deleting a confirmation popup ( :numref:`image142` ) is displayed, which requires the user to confirm if the action should really be carried out?

      .. _image142:
      .. figure:: /img/user_manual/claim.delete_conf.png
        :align: center

        `Delete confirmation – Claims Control Page`


 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a claim has been added, updated or deleted or if there was an error at any time during the process of these actions.

.. _claim-page:

Claim Page
""""""""""

 #. **Data Entry**

    .. _claim_add_img:
    .. figure:: /img/user_manual/claim.add.png
      :align: center

      `Claim Page`


    * ``HF Code``

      Displays the code of the health facility. The field is read only (taken over from the :ref:`Claims Control Page  <health_facility_claims>`) and cannot be edited.

    * ``HF Name``

      Displays the name of the health facility. The field is read only (taken over from the :ref:`Claims Control Page  <health_facility_claims>`) and cannot be edited.

    * ``Insurance Number``

      Enter the insurance number of the patient. When the field is selected, the search insuree popup(:refnum:'insuree_picker') will be display and will allow the claim administrator to search the insuree based on its insurance number, or/and last name, or/and other(first) name . Mandatory.

      .. _insuree_picker:
      .. figure:: /img/user_manual/insuree_picker.png
        :align: center

        `Search insuree popup`

    * ``Claim No.``

      Enter the identification of the claim. Mandatory, up to 8 characters. It should be unique within the claiming health facility.

    * ``Main Dg.``

      Select the code of the main diagnosis by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box. Mandatory.

    * ``Sec Dg 1``

      Select the code of the first secondary diagnosis by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box.

    * ``Sec Dg 2``

      Select the code of the second secondary diagnosis by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box

    * ``Sec Dg 3``

      Select the code of the third secondary diagnosis by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box

    * ``Sec Dg 4``

      Select the code of the fourth secondary diagnosis by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box
    * ``Claim Administrator``

      Displays code of the claim administrator. The field is read only (taken over from :ref:`the Claim Control Page  <health_facility_claims>`) and cannot be edited.

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

      #. ``service code``

        When entering the service code, a dropdown suggestion box for the available services with the service code or service name matching your typed text will be shown. Available medical services in the dropdown suggestion box are taken over from the pricelist of medical services associated with the claiming health facility. The desired service can then be selected from the dropdown suggestion box by clicking on it using mouse or selecting it using up and down arrows, then pressing Enter key fill the service code text field, together with quantity and value field in the same row.

        Once the selected service has been written on the service data grid row, a new service line will be added and the dropdown suggestion box will close itself. When needed, the dropdown suggestion box can be closed by clicking any place on the page but outside the dropdown suggestion box.

        .. _image144:
        .. figure:: /img/user_manual/image117.png
          :align: center

          `Services dropdown suggestion box – Claim Page`

      #. ``quantity``

        This field can be filled manually by entering a number in it or automatically is filled by 1 when the service code above is filled, through dropdown suggestion box. It is this field that receives focus after service code is filled above from the dropdown suggestion box.

      #. ``price``

        This field can be filled manually by entering a number in it or automatically is filled when the service code above is filled, through dropdown suggestion box. Automatically filled prices are taken over from the pricelist of medical services associated with the claiming health facility.

      #. ``explanation``

        Enter extra information about the service for the scheme administration (a medical officer of the scheme administrator).

    * ``Items``

      #. ``item code``

        When entering the item code, a dropdown suggestion box for the available items with the item code or item name matching your typed text will be shown. Available medical items in the dropdown suggestion box are taken over from the pricelist of medical items associated with the claiming health facility. The desired item can then be selected from the dropdown suggestion box by clicking on it using mouse or selecting it using up and down arrows, then pressing Enter key to fill the item code text field, together with quantity and value field in the same row.


        Once the selected item has been written on the item data grid row, a new service line will be added and the dropdown suggestion box will close itself. When needed, the dropdown suggestion box can be closed by clicking any place on the page but outside the dropdown suggestion box.

        .. _image145:
        .. figure:: /img/user_manual/image118.png
          :align: center

          `Items dropdown suggestion box – Claim Page`

      #. ``quantity``

        This field can be filled manually by entering a number in it or automatically is filled by 1 when the item code above is filled, through dropdown suggestion box. It is this filled that receives focus after item code is filled above from the dropdown suggestion box.

      #. ``price``

        This field can be filled manually by entering a number in it or automatically is filled when the item code above is filled, through dropdown suggestion box. Automatically filled prices are taken over from the pricelist of medical items associated with the claiming health facility.

      #. ``explanation``

        Enter extra information about the medical item for the scheme administration (a medical officer of the scheme administrator).

    * ``claimed``

      This field is filled automatically with a new total of quantities multiplied to their corresponding values in both data input grids at any time when there is a change in values in the either quantity fields or value fields anywhere in both data input grids.

    * ``explanation``

      Enter extra information about the whole claim for the scheme administration (a medical officer of the scheme administrator).


 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button (:numref:`mat_save`) will save the claim. The user stay in the :ref:`Claim Page  <claim-page>`; a message confirming that the claim has been saved will appear on the right of the :ref:`Claim Page  <claim-page>` (:numref:`save_conf`).

    .. _save_conf:
    .. list-table:: claim save confirmation

      * - .. figure:: /img/user_manual/claim.create_conf.png
            :align: center

            `Create confirmation`
        - .. figure:: /img/user_manual/claim.save_conf.png
            :align: center

            `Update confirmation`

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk).

 #. **Printing of a claim**

    By clicking on the ``Print`` button (:numref:`mat_print`), the user will be shown a printable version of the claim details page. The printable version of the claim is available in the pdf formats.

 #. **Creating of a new claim**

    By clicking on the ``Add`` button (:numref:`mat_add`), the :ref:`Claim Page  <claim-page>` is cleared (with exception of HF Code, HF Name and Claim Administrator) and it ready for entering of a new claim for the same health facility and of the same claim administrator as before.

 #. **back**

      By clicking on the ``back`` (:numref:`mat_back`) button, the user will be re-directed to the :ref:`Claims Control Page  <health_facility_claims>`.
