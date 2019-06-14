Review claims
^^^^^^^^^^^^^

  The functionality allows reviewing and adjustments of claims from medical point of view. Reviewing of claims is restricted to users with the system role of Medical Officer or with a role including an access to Claims/Claim/Review.

Pre-conditions
""""""""""""""

  A claim has been already submitted.

Navigation
""""""""""

  All functionality for use with the administration of claim overview can be found under the main menu ``Claims``, sub menu ``Review.``

  .. _image150:
  .. figure:: /img/user_manual/image123.png
    :align: center

    `Image 150 - Navigation Review`

  Clicking on the sub menu ``Review`` re-directs the current user to the `Claims Overview Page. <#claims-overview-page>`__

  .. _claims_review_img:
  .. figure:: /img/user_manual/claims_review_page.png
    :align: center

    `Image - Claims Overview Page`

Claims Overview Page
""""""""""""""""""""

  The Claims Overview Page is the central point for all claim review administration. By having access to this panel, it is possible to review, feedback, amend and process claims. The panel is divided into five sections (:ref:`Image 150<image150>`).

 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. In the case of claims the following search options are available, which can be used alone, or in combination with each other.

    * ``Region``

      Select the ``Region``; where searched for health facility is located or where patients are permanently living from the list of regions by clicking on the arrow on the right of the selector to select claims from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected*

    * ``District``

      Select the ``District``; where searched for health facility is located or where patients are permanently living from the list of districts by clicking on the arrow on the right of the selector to select claims from a specific district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected.*

    * ``HF Code``

      Select the ``HF Code``; from the list of health facilities codes by clicking on the arrow on the right of the selector to select claims from a specific health facility. *Note: The list will only be filled with the health facilities belonging to the selected district and assigned to the current logged in user.*

    * ``HF Name``

      Type in the beginning of; or the full ``HF Name``, to search for claims belonging to the health facility whose name start with or match completely the typed text.

    * ``Claim Administrator``

      Select the ``claim administrator`` from the list of claim administrator codes by clicking on the arrow on the right of the selector, to select claims submitted by a specific claim administrator. *Note: The list will only be filled with the claim administrators belonging to the health facility selected.*

    * ``Insurence Number``

      Type in the beginning of; or the full ``Insurence Number``, to search for claims for patients with the insurance number which start with or match completely the typed text.

    * ``Claim No.``

      Type in the beginning of; or the full ``Claim No.``, to search for claims with claim identification which start with or match completely the typed text.

    * ``Review Status``

      Select the ``Review Status`` from the list of the options for review status by clicking on the arrow on the right of the selector, to select claims with a specific review status.

    * ``Feedback Status``

      Select the ``Feedback Status`` from the list of the options for feedback status by clicking on the arrow on the right of the selector, to select claims with a specific feedback status.

    * ``Claim Status``

      Select the ``Claim Status`` from the list of options for claim status by clicking on the arrow on the right of the selector, to select claims with a specific claim status.

    * ``Main Dg``

      Select the ``Main Dg.`` from the list of diagnoses status by typing text, all diagnoses containing the typed text will appear and be selectable underneath the box, to select claims with main diagnosis.

    * ``Batch Run``

      Select the ``Batch Run`` from the list of batch runs by clicking on the arrow on the right of the selector, to select claims included in a specific batch run.

    * ``Visit Date From``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Visit Date From`` which is on or is greater than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Visit Date To``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Visit Date To`` which is on or is less than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Claim Date From``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Claim Date From`` which is on or is greater than the  date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Claim Date To``

      Type in a date; or use the Date Selector Button, to search for claims with a ``Claim Date To`` which is on or is less than the date typed/selected. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Visit Type``

      Select type of out-patient visit or in-patient admission from the list of types of visit to search for claims made on specific visit/admission type.

    * ``Date Selector Button``

      Clicking on the Date Selector Button will pop-up an easy to use, calendar selector (:ref:`Image 152<image152>`); by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

        - At anytime during the use of the pop-up, the user can see the date of **today**.
        - Clicking on today will close the pop-up and display the today’s date in the corresponding date entry box.
        - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
        - Clicking on the arrow to the left displays the previous month.
        - Clicking on the arrow on the right will displays the following month.
        - Clicking on the month will display all the months for the year.
        - Clicking on the year will display a year selector.

      .. _image152:
      .. |logo39| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo40| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo41| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +----------++----------++----------+
      | |logo39| || |logo40| || |logo41| |
      +----------++----------++----------+

        `Image 152 - Calendar Selector - Search Panel`

    * ``Search Button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the Result Panel.

 #. **Claim Selection Update Panel**

    This panel is basically for functionality of updating multiple claims which are currently loaded in the Result Panel at once basing on the claim filter criteria available on this panel. The update on the claims is basically changing **Feedback Status** and **Review Status** of a claim from **Idle** to (**Not**) **Selected for Feedback** or (**Not**) **Selected for Review** respectively. The filters in this panel work on the claims which are currently loaded on the result panel. The combination of filters is either ``Select`` alone or ``Select`` and either ``Random`` or ``Value`` or ``Variance`` or combination of ``Value`` and ``Variance``.

    * ``Select``

      A selection dropdown box to select between **Review Select** and **Feedback Select** to filter only claims whose review status is **Idle** or feedback status is **Idle** respectively from among claims currently in the Result Panel.

    * ``Random``

      Accept a number which is considered to be a percentage of the claims in the Result Panel. Check the random checkbox and enter a number on the text field next to checkbox. The default is 5%.

    * ``Value``

      Accept a number which is considered to be claimed value. This will filter claims from the Result Panel by taking claims whose claimed value is equal or greater than the entered number in the Value text field. Check the value checkbox and enter a number on the text field next to checkbox. The default is 40000.

    * ``variance``

      Accept a number which is considered to be a percentage of the current claim value variance. Calculated by dividing the current claim value **(value)** and the average sum **(Average)** of the all claims in the previous year from the current claim date and with the same main diagnosis as that of the current claim, minus one **(1)** and finally multiply by hundred **(100)** to get the percentage variance. I.e **Percentage Variance = [(Value / Average) – 1] \* 100** Enter a number by checking the variance checkbox and enter a number on the text field next to checkbox. The default is 50%.

    * ``Update button``

      Once desired criteria have been set and after clicking this button, then the claims currently displayed in the result panel which satisfy the criteria, will be updated of their **Idle** Review Status or Feedback Status to either (**Not**) **Selected for Review** or (**Not**) **Selected for Feedback** respectively.


      A popup prompt window will be displayed to confirm the process, as shown on (:ref:`Image 153<image153>`) and (:ref:`Image 154<image154>`).


      Once the update process is over, a popup window (:ref:`Image 155<image155>`). Showing the result of the process will be displayed.

      .. _image153:
      .. figure:: /img/user_manual/image125.png
        :align: center

        `Image 153 - Claim Feedback Selection Update Prompt – Claims Overview Page`

      .. _image154:
      .. figure:: /img/user_manual/image126.png
        :align: center

        `Image 154 - Claim Review Selection Update Prompt – Claims Overview Page`

      .. _image155:
      .. figure:: /img/user_manual/image127.png
        :align: center

        `Image 155 - Claim Selection Update Results – Claims Overview Page`

 #. **Result Panel**

    The Result Panel displays a list of all claims found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 156<image156>`).

    .. _image156:
    .. figure:: /img/user_manual/image128.png
      :align: center

      `Image 156 - Selected record (blue), hovered records (yellow) - Result Panel`

    A maximum of 2000 records can be displayed at one time, in a scroll panel. Further records can be viewed by processing the current loaded claims and search claims again.


    The Feedback and Review Status Columns in each row contain a drop down list with options for claim feedback status and claim review status. A user can change the claim feedback and review status from low status to high status only. Either from **Idle** to **Not Selected** or **Selected for Feedback** in case of the feedback status or **Not Selected** or **Selected for Review** in case of the review status. Or from **Not Selected** to **Selected for Feedback** in case of the feedback status or **Selected for Review** in case of the review status. For changes to take effect, a user will have to update the changes by clicking the ``Update`` button.

 #. **Button Panel**

    With exception of the Cancel button, which re-directs to the `Claims Overview Page <#claims-overview-page>`__, the button panel is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record.

    * ``review``

      Clicking on this button re-directs a user to the `Claim Review Page <#claim-review-page>`__, where a claim with review status **Selected for Review** can be reviewed and its current review status changed to **Reviewed.** If the claim is not in the status **Selected for Review** then the claim can be only loaded and shown to the user without any subsequent action.


      The page will open with the current information loaded into the data entry fields. See the `Claim Review Page <#claim-review-page>`__, for information on the data entry and mandatory fields.

    * ``feedback``

      Clicking on this button re-directs a user to the `Claim Feedback Page <#claim-feedback-page>`__, where a claim with feedback status **Selected for Feedback** can be feed backed and its current feedback status changed to **Delivered**.


      The page will open with the current information loaded into the data entry fields. See the `Claim Feedback Page <\l>`__ for information on the data entry and mandatory fields.

    * ``update``

      Clicking on this button, update the feedback status and review status of claims in the result panel from either **Idle** to **Not Selected** or **Selected for Feedback** or **Selected for Review** respectively or from **Not Selected** to **Selected for Feedback** or **Selected for Review** respectively.

    * ``process``

      Clicking on this button changes the claim status **Checked** of all current selected claims in the Result Panel, selected by checking the checkbox on the right end of each record, to claim status **Processed**.


      Claims which can be selected for being processed are ones whose claim status is **Checked** and **Feedback Status** and **Review Status** are not **Idle**. The checkbox on the top of the Result Panel can be used to select multiple claims. The process happens while a user stays on the same page. Once the process is done, a popup window (:ref:`Image 157<image157>`) showing results of the process will be shown.

      .. _image157:
      .. figure:: /img/user_manual/image129.png
        :align: center

        `Image 157 - Process Claim Prompt – Claims Overview Page`

      .. _image158:
      .. figure:: /img/user_manual/image130.png
        :align: center

        `Image 158 - Processed Claims details – Claims Overview Page`

    * ``Cancel``

      By clicking on the cancel button, the user will be re-directed to the `Claims Overview Page <#claims-overview-page>`__.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a claim has been reviewed, updated, feedback added on claim or if there was an error at any time during the process of these actions.

Claim Review Page
"""""""""""""""""

 #. **Data Entry**

    .. _image159:
    .. figure:: /img/user_manual/image131.png
      :align: center

      `Image 159 - Claim Review Page`


      ``Claim Review Page`` will show read-only information of the current claim selected for review, on the top section of the page, on some of the grid columns of the claim services grid and claim items grid and on the bottom of all the grids. As well, the page has input boxes where a user with the system role Medical Officer or with a role including an access to Claims/Claim/Review can enter new relevant values for review of the current claim.


      Read-only information of the current claim includes the following:

    * ``HF``

      The health facility code and name which the claim belongs to.

    * ``Main Dg.``

      The code of the main diagnosis.

    * ``Sec Dg1``

      The code of the first secondary diagnosis.

    * ``Sec Dg2``

      The code of the second secondary diagnosis.

    * ``Sec Dg3``

      The code of the third secondary diagnosis.

    * ``Sec Dg4``

      The code of the fourth secondary diagnosis.

    * ``Visit type``

      The type of the visit or of the hospital stay (**Emergency, Referral, Other**)

    * ``Date Processed``

      The date on which the claim was processed (sent to the state **Processed**).

    * ``Claim Administrator``

      The administrator's code, who was responsible for submission of the current claim.

    * ``Insurance Number``

      The insurance number of the patient.

    * ``Claim No.``

      The unique identification of the claim within the claiming health facility.

    * ``Patient Name``

      The full name of the patient on whom the claim is made.

    * ``Date Claimed``

      The date on which the claim was prepared by the claiming health facility.

    * ``Visits Date From``

      The date on which the patient visited (or was admitted by) the health facility for treatment on which the claim is basing on.

    * ``Visit Date To``

      The date on which the patient was discharged from the health facility for treatment on which the claim is basing on.

    * ``Guarantee No.``

      Identification of a guarantee letter.

    * ``Claimed``

      The sum of prices of all claimed services and items at the moment of submission of the claim.

    * ``approved``

      The value of the claim after automatic checking during its submission and after the corrections of the claim done by a medical officer.

    * ``Adjusted``

      The value of the claim after automatic adjustments done according to the conditions of coverage by the patient’s policy.

    * ``Explanation``

      Explanation to the claim provided by the claiming health facility.

    * ``claim status``

      Claim status is shown on the very bottom right end side after the two grids. This is status which claim gets after submission.

    * ``Adjustment``

      Enter a text summarizing adjustments in claim done by a medical officer.

    * **Services and Items data entry grids.**

      #. ``Approved Quantity (app.qty)``

         Enter a number of approved provisions of the corresponding medical service or item.

      #. ``Approved Price (app. price)``

         Enter an approved price of the corresponding medical service or item.

      #. ``justification``

         Enter justification for the entered corrections of the price and quantity of the medical service or item.

      #. ``status``

         Select either the status in the claim **Passed** or **Rejected** for the corresponding medical service or item respectively.

      #. ``rejection reason``

         The last column of each of the two grids, headed with character  '**R**', gives rejection reason number for each of the claimed services or claimed items in the claim services grid or the claim items grid respectively. Rejection reasons are as follows:

         The rejection description is displayed on the screen when the mouse pointer is above the given line (:ref:`Image Rejection Description <rejection_desk_img>`)

         .. _rejection_desk_img:
         .. figure:: /img/user_manual/rejection_desc.png
            :align: center

            `Image  Rejection Description`

        +-----------------------------------+-----------------------------------+
        | Reason Code                       | Reason Description                |
        +===================================+===================================+
        | -1                                | Rejected by a medical officer     |
        +-----------------------------------+-----------------------------------+
        | 0                                 | Accepted                          |
        +-----------------------------------+-----------------------------------+
        | 1                                 | Item/Service not in the registers |
        |                                   | of medical items/services         |
        +-----------------------------------+-----------------------------------+
        | 2                                 | Item/Service not in the           |
        |                                   | pricelists associated with the    |
        |                                   | health facility                   |
        +-----------------------------------+-----------------------------------+
        | 3                                 | Item/Service is not covered by an |
        |                                   | active policy of the patient      |
        +-----------------------------------+-----------------------------------+
        | 4                                 | Item/Service doesn’t comply with  |
        |                                   | limitations on patients           |
        |                                   | (men/women, adults/children)      |
        +-----------------------------------+-----------------------------------+
        | 5                                 | Item/Service doesn’t comply with  |
        |                                   | frequency constraint              |
        +-----------------------------------+-----------------------------------+
        | 6                                 | Item/Service duplicated           |
        +-----------------------------------+-----------------------------------+
        | 7                                 | Not valid insurance number        |
        +-----------------------------------+-----------------------------------+
        | 8                                 | Diagnosis code not in the current |
        |                                   | list of diagnoses                 |
        +-----------------------------------+-----------------------------------+
        | 9                                 | Target date of provision of       |
        |                                   | health care invalid               |
        +-----------------------------------+-----------------------------------+
        | 10                                | Item/Service doesn’t comply with  |
        |                                   | type of care constraint           |
        +-----------------------------------+-----------------------------------+
        | 11                                | Maximum number of in-patient      |
        |                                   | admissions exceeded               |
        +-----------------------------------+-----------------------------------+
        | 12                                | Maximum number of out-patient     |
        |                                   | visits exceeded                   |
        +-----------------------------------+-----------------------------------+
        | 13                                | Maximum number of consultations   |
        |                                   | exceeded                          |
        +-----------------------------------+-----------------------------------+
        | 14                                | Maximum number of surgeries       |
        |                                   | exceeded                          |
        +-----------------------------------+-----------------------------------+
        | 15                                | Maximum number of deliveries      |
        |                                   | exceeded                          |
        +-----------------------------------+-----------------------------------+
        | 16                                | Maximum number of provisions of   |
        |                                   | item/service exceeded             |
        +-----------------------------------+-----------------------------------+
        | 17                                | Item/service cannot be covered    |
        |                                   | within waiting period             |
        +-----------------------------------+-----------------------------------+
        | 18                                | N/A                               |
        +-----------------------------------+-----------------------------------+
        | 19                                | Maximum number of antenatal       |
        |                                   | contacts exceeded                 |
        +-----------------------------------+-----------------------------------+

 #. **Saving**

    Once appropriate data is entered, clicking on the ``Save`` button will save the claim. The user will be re-directed back to the `Claims Overview Page <#claims-overview-page>`__\; a message confirming that the claim has been saved will appear on the Information Panel. The ``Save`` button appears only if the claim was reviewed in the status **Selected for Review.**

 #. **reviewing**

    Once appropriate data is entered, clicking on the ``Reviewed`` button will save the claim and change the claim Review Status from **Selected for Review** to **Review**. The user will be re-directed back to the `Claims Overview Page <#claims-overview-page>`__\; a message confirming that the claim has been saved will appear on the Information Panel. The ``Reviewed`` button appears only if the claim was reviewed in the status **Selected for Review**.

 #. **data entry validation**

    If inappropriate data is entered at the time the user clicks the ``Save`` or `` review`` button, an error message will appear in the Information Panel, and the data field will take the focus.

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Claims Overview Page <#claims-overview-page>`__.

Claim Feedback Page
"""""""""""""""""""
    The Claim Feedback page will show read-only information of the current claim selected for feedback, on the top section of the page it has input boxes where a user with the system role Medical Officer or with a role including an access to Claims/Claim/Feedback can enter feedback on the current claim or where the user can read a feedback delivered by enrolment officers.

 #. **Data Entry**

    .. _image160:
    .. figure:: /img/user_manual/image132.png
      :align: center

      `Image 160 - Claim Feedback Page`

   Read-only data of the feedback includes in the section **Claim** the following:

    * ``HF Code``

      The health facility code which the claim belongs to.

    * ``HF Name``

      The health facility name which the claim belongs to.

    * ``Claim Administrator``

      The administrator's code, who was responsible for submission of the current claim.

    * ``Insurance Number``

      The insurance number of the patient.

    * ``Claim No.``

      The unique identification of the claim within the claiming health facility.

    * ``Last Name``

      The last name of the patient on whom the claim is made.

    * ``Other Names``

      The other names of the patient on whom the claim is made.

    * ``Date Claimed``

      The date on which the claim was prepared by the claiming health facility.

    * ``Visits Date From``

      The date on which the patient visited (or was admitted by) the health facility for treatment on which the claim is basing on.

    * ``Visit Date To``

      The date on which the patient was discharged from the health facility for treatment on which the claim is basing on.

    * ``Review Status``

      The status of the claim with respect to reviewing.

    * ``Feedback Status``

      The status of the claim with respect to feed backing.

   Modifiable data of the feedback included in the section **Feedback** the following

    * ``Enrolment Officer``

      Select an enrolment officer from the list of enrolment officers, by clicking the arrow on the right side of selection field. The enrolment officer collects feedback from the patient.

    * ``Care Rendered``

      Select ‘Yes’ or ‘No’ from the list, by clicking the arrow on the right side of selection field.

    * ``Payment Asked``

      Select ‘Yes’ or ‘No’ from the list, by clicking the arrow on the right side of selection field.

    * ``Drugs Prescribed``

      Select ‘Yes’ or ‘No’ from the list, by clicking the arrow on the right side of selection field.

    * ``Drugs Received``

      Select ‘Yes’ or ‘No’ from the list, by clicking the arrow on the right side of selection field

    * ``Overall Assessment``

      Choose one level among the six levels available by checking/clicking on the desired checkbox.

    * ``Feedback Date``

      Type in a date of collection of the feedback; or use the date selector button, to enter date. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the back space key.*

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 161<image161>`); by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

        - At anytime during the use of the pop-up, the user can see the date of **today**.
        - Clicking on today will close the pop-up and display the today’s date in the corresponding date entry box.
        - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
        - Clicking on the arrow to the left displays the previous month.
        - Clicking on the arrow on the right will displays the following month.
        - Clicking on the month will display all the months for the year.
        - Clicking on the year will display a year selector.

      .. _image161:
      .. |logo42| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo43| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo44| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +----------++----------++----------+
      | |logo42| || |logo43| || |logo44| |
      +----------++----------++----------+

        `Image 161 - Calendar Selector - Search Panel`

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the feedback on current claim. The user will be re-directed back to the `Claims Overview Page <#claims-overview-page>`__\ ; a message confirming that the feedback has been saved will appear on the Information Panel. If inappropriate data is entered or mandatory data is not entered at the time the user clicks the Save button, an error message will appear in the Information Panel, and the data field will take the focus.

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Claims Overview Page <#claims-overview-page>`__\ .
