Insurance Products Administration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  The register of insurance products contains all insurance products in the health insurance scheme. There may be several insurance products available for distribution/selling in a territory, e.g. one basic product and one or several supplemental insurance products. The insurance products may at the different levels. For example that basic insurance product may be at the national level whereas the supplemental insurance products may be at the regional level. Administration of the register of insurance products is restricted to users with the role of Scheme Administrator.

Pre-conditions
""""""""""""""

  An insurance product may only be added or thereafter edited, after the approval of the management of the scheme administration.

Navigation
""""""""""

  All functionality for use with the administration of insurance products can be found under the main menu ``Administration``, sub menu ``Products``.

  .. _image4:
  .. figure:: /img/user_manual/image4.png
    :align: center

    `Image 4 - Navigation Products`

Product Control Page
""""""""""""""""""""

  Clicking on the sub menu ``Products`` re-directs the current user to the ``Product Control Page``.

  .. _image5:
  .. figure:: /img/user_manual/image5.png
    :align: center

    `Image 5 - Product Control Page`

  The ``Product Control Page`` is the central point for administration of insurance products. By having access to this page, it is possible to add, edit, duplicate and search. The panel is divided into four panels. (:ref:`Image 5<image5>`)

 #. **Search Panel**

    The search panel allows a user to select specific criteria to minimise the search results. In the case of Products the following search options are available, which can be used alone, or in combination with each other.

    * ``Product Code``

      Type in the beginning of; or the full ``Product Code``; to search for products with a ``Product Code``, which starts with or matches completely, the typed text.

    * ``Product Name``

      Type in the beginning of; or the full ``Product Name`` to search for products with a ``Product Name``, which starts with or matches completely, the typed text.

    * ``Date From``

      Type in a date; or use the Date Selector Button, to search for products with a ``Date From``, which is on or is greater than the date typed/selected. *Note: To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Date To``

      Type in a date; or use the Date Selector Button, to search for products with a ``Date To``, which is on or is greater than the date typed/selected. *Note: To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 6<image6>`); by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

      - Anytime during the use of the pop-up, the user can see the date of today.

      - Clicking on today will close the pop-up and display the today’s date in the corresponding date entry box.

      - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.

      - Clicking on the arrow to the left displays the previous month.

      - Clicking on the arrow on the right will displays the following month.

      - Clicking on the month will display all the months for the year.

      - Clicking on the year will display a year selector.

      .. _image6:
      .. |logo1| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo2| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo3| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +---------+---------+---------+
      | |logo1| | |logo2| | |logo2| |
      +---------+---------+---------+

        `Image 6 - Calendar Selector - Search Panel`

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select products from a specific region. The option **National** means that the found insurance products should be common for all regions. `Note: The list will only be filled with the regions assigned to the current logged in user and with the option National. All nationwide products and all regional products relating to the selected region will be found. If no district is selected then also all district products for districts belonging to the selected region will be found.`

    * ``District``

      Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to select products from a specific district. `Note: The list will be only filled with the districts belonging to the selected region. All nationwide products, all regional products relating to the selected region and all district products for the selected district will be found.`

    * ``Historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in the result with a line through the middle of the text (strikethrough) to clearly define them from current records (:ref:`Image 7<image7>`).

      .. _image7:
      .. figure:: /img/user_manual/image9.png
        :align: center

        `Image 7 - Historical records - Result Panel`

    * ``Search Button``

      Once the criteria have been entered, use the search button to filter the records, the results will appear in the result panel.

 #. **Result Panel**

    The result panel displays a list of all products found, matching the selected criteria in the search panel. The currently selected record is highlighted with light blue, while hovering over records changes the highlight to yellow (:ref:`Image 8<image8>`). The leftmost record contains a hyperlink which if clicked, re-directs the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

    .. _image8:
    .. figure:: /img/user_manual/image10.png
      :align: center

      `Image 8 - Selected record (blue), hovered records (yellow) - Result Panel`

    A maximum of 15 records are displayed at one time, further records can be viewed by navigating through the pages using the page selector at the bottom of the result Panel (:ref:`Image 9<image9>`).

    .. _image9:
    .. figure:: /img/user_manual/image11.png
      :align: center

      `Image 9 - Page selector - Result Panel`

 #. **Button Panel**

    With exception of the ``Cancel`` button, which re-directs to the Home Page (:ref:`Image 2<image2>`), and the Add button which re-directs to the product page, the button panel (the buttons ``Edit`` and ``Duplicate`` ) is used in conjunction with the current selected record (highlighted with blue). The user should first select a record by clicking on any position of the record except the leftmost hyperlink, and then click on the button.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a product has been added, updated or deleted or if there was an error at any time during the process of these actions.

Product Page
""""""""""""

 #. **Data Entry**

    .. _image10:
    .. |logo4| image:: /img/user_manual/image12.png
      :scale: 100%
      :align: middle
    .. |logo5| image:: /img/user_manual/image13.png
      :scale: 100%
      :align: middle

    +---------+
    | |logo4| |
    +---------+
    | |logo5| |
    +---------+

      `Image 10 - Product Page`

    * ``Product Code``

      Enter the product code for the product. Mandatory, 8 characters.

    * ``Product Name``

      Enter product name for the product. Mandatory, 100 characters maximum.

    * ``Region``

      Select the region in which the product will be used, from the list by clicking on the arrow on the right hand side of the lookup. The option National means that the insurance product is nationwide and it is not constraint to a specific region. `Note: The list will only be filled with the regions assigned to the current logged in user and with the option National.` Mandatory.

    * ``District``

      Select the district in which the product will be used, from the list by clicking on the arrow on the right hand side of the lookup. `Note: The list will only be filled with the districts assigned to the selected region and assigned to the current logged in user. If no district is selected then the product is considered to be either nationwide (the option National is selected in the field Region) or regional associated with the selected region.`

    * ``Date From``

      Type in the date or use the ``Date Selector Button`` to provide the date for which underwriting for the insurance product can be done from. ``Date From`` determines the earliest date from which underwriting can be done. `Note: To clear the date entry box; use the mouse to highlight the full date and then press the space key.` Mandatory.

    * ``Date To``

      Type in the date or use the Date Selector Button to provide the date until which underwriting can be done to.`Note: To clear the date entry box; use the mouse to highlight the full date and then press the space key.` Mandatory.

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 11<image11>`). By default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted. At anytime during the use of the pop-up, the user can see the date of ``today``.

      - Clicking on ``today`` will close the pop-up and display the today’s date in the corresponding date entry box.
      - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
      - Clicking on the arrow to the left displays the previous month.
      - Clicking on the arrow on the right will displays the following month.
      - Clicking on the month will display all the months for the year.
      - Clicking on the year will display a year selector.

      .. _image11:
      .. |logo6| image:: /img/user_manual/image6.png
        :scale: 100%
        :align: middle
      .. |logo7| image:: /img/user_manual/image7.png
        :scale: 100%
        :align: middle
      .. |logo8| image:: /img/user_manual/image8.png
        :scale: 100%
        :align: middle

      +---------+---------+---------+
      | |logo6| | |logo7| | |logo8| |
      +---------+---------+---------+

        `Image 11 - Calendar Selector - Search Panel`

    * ``Conversion``

      Select from the list of products, a reference to the product which replaces the current product in case of renewal after the ``Date to``. `Note: Selecting the current product will prevent the record from saving, and cause a message to be displayed in the Information Panel.`

    * ``Lump Sum``

      Enter the lump sum contribution (an amount paid irrespective of the number of members up to a threshold) to be paid by a household/group for the product. If the lump sum is zero no lump sum is applied irrespective of the threshold members. Decimal up to two digits.

    * ``Threshold Members``

      Enter the threshold number of members in product for which the lump sum is valid.

    * ``Number of Members``

      Enter the maximal number of members of a household/group for the product.

    * ``Contribution Adult``

      Enter the contribution to be paid for each adult (on top of the threshold number of members). Decimal up to two digits.

    * ``Contribution Child``

      Enter the contribution to be paid for each child (on top of the threshold number of members). Decimal up to two digits.

    * ``Insurance Period``

      Enter duration of the period in months, in which a policy with the product will be valid. Mandatory.

    * ``Administration Period``

      Enter duration of the administration period in months. The administration period is added to the enrolment date/renewal date for determination of the policy start date.

    * ``Max Instalments``

      Enter maximal number of instalments in which contributions for a policy may be paid. Mandatory.

    * ``Grace Period Payment``

      Enter duration of the period in months, in which a policy has a grace period (not fully paid up) before it is suspended. Mandatory, although it is by default and can be left at zero.

    * ``Grace Period Enrolment``

      Enter duration of the period in months after the starting date of a cycle (including this starting date), in which underwriting of a policy will still be associated with this cycle.

    * ``Grace Period Renewal``

      Enter duration of the period in months after the starting date of a cycle (including this starting date), in which renewing of a policy will still be associated with this cycle.

    * ``Enrolment Discount percentage``

      Enter the enrolment discount percentage for the insurance product. The discount percentage is applied on the total contributions calculated for a policy underwritten earlier than ``Enrolment disc. period`` months before the start date of the corresponding cycle.

    * ``Enrolment Discount Period``

      Enter the enrolment discount period of the insurance product in months.

    * ``Renewal Discount Percentage``

      Enter the renewal discount percentage for the insurance product. The discount percentage is applied on the total contributions calculated for a policy renewed earlier than ``renewal disc. period`` months before the start date of the corresponding cycle.

    * ``Renewal Discount Period``

      Enter the renewal discount period of the insurance product in months.

    * ``Medical Services``

      Select from the list of available medical services (from the register of Medical Services) the medical services covered within the insurance product, by either clicking on the ``Check All`` box at the top of the list of medical services, or by selectively clicking on the check box to the left of the medical service.

    * ``Medical Services Grid``

      .. _image 12:
      .. figure:: /img/user_manual/image14.png
        :align: center

        `Image 12 - Medical Services - Product`

    * ``Code``

      Displays the code for the medical service

    * ``Name``

      Displays the name of the medical service

    * ``Type``

      Displays the type of the medical service

    * ``Level``

      Displays the level of the medical service

    * ``Limit``

      Indicates the type of limitation of coverage for the medical service. This may be adjusted per medical service, select between Co-Insurance [C] and Fixed amount [F]. Co-insurance means coverage of a specific percentage of the price of the medical service by policies of the insurance product. Fixed amount means coverage up the specified limit. C is the default value. Limit O is used for claims having the type of visit Other, Limit R is used for claims having the type of visit Referral and Limit E is used for claims having the type of visit Emergency.

    * ``Origin``

      Indicates where the price for remuneration of the service comes from. This may be adjusted per service, the options are: [P] Price taken from the price list of a claiming health facility, [O] Price taken from a claim and [R] Relative price, the nominal value of which is taken from the price list and the actual value of which is determined backwards according to available funds and volume of claimed services and medical items in a period. [R] is the default value.

    * ``Adult``

      Indicates the limitation for adults. If the type of limitation is a co-insurance then the value is the percentage of the price covered by policies of the insurance product for adults. If the type of limitation is a fixed limit the value is an amount up to which price of the service is covered for adults by policies of the insurance product. Default is 100%. Adult O is for Other, Adult R is for Referral and Adult E is for Emergency claims according to the type of visit (Visit Type).

    * ``Child``

      Indicates the limitation for children. If the type of limitation is a co-insurance then the value is the percentage of the price covered for children by policies of the insurance product. If the type of limitation is a fixed limit the value is an amount up to which price of the service is covered for children by policies of the insurance product. Default is 100%. Child O is for Other, Child R is for Referral and Child E is for Emergency claims according to the type of visit (Visit Type).

    * ``No Adult``

      It indicates the maximal number of provisions of the medical service during the insurance period for an adult.

    * ``No Child``

      It indicates the maximal number of provisions of the medical service during the insurance period for an child.

    * ``Waiting Period Adult``

      Indicates waiting period in months (after the effective date of a policy) for an adult.

    * ``Waiting Period Child``

      Indicates waiting period in months (after the effective date of a policy) for a child.

    * ``Ceiling Adult``

      It indicates whether the medical service is excluded from comparison against ceilings defined in the insurance product for adults. Default is that the medical service is not excluded from comparisons with ceilings. [H] means exclusion only for provision of in-patient care, [N] means exclusion only for out-patient care and [B] means exclusion both for in-patient and out-patient care.

    * ``Ceiling Child``

      It indicates whether the medical service is excluded from comparison against ceilings defined in the insurance product for children. Default is that the medical service is not excluded from comparisons with ceilings. [H] means exclusion only for provision of in-patient care, [N] means exclusion only for out-patient care and [B] means exclusion both for in-patient and out-patient care.

    * ``medical items``

      Select from the list of available medical items (from the register of Medical Items) the medical items covered within the product; by either clicking on the Check All box at the top of the list of medical items, or by selectively clicking on the check box to the left of the medical item.

    * ``medical items grid``

      .. _image 13:
      .. figure:: /img/user_manual/image15.png
        :align: center

        `Image 13 - Medical Items - Product`

    * ``Code``

      Displays the code for the medical item

    * ``Name``

      Displays the name of the medical item

    * ``Type``

      Displays the type of the medical item

    * ``Package``

      Displays the packaging of the medical Item

    * ``Limit``

      Indicates the type of limitation of coverage for the medical item. This may be adjusted per medical item, select between Co-Insurance [C] and Fixed amount [F]. Co-insurance means coverage of a specific percentage of the price of the medical item by policies of the insurance product. Fixed amount means coverage up the specified limit. C is the default value. Limit O is used for claims having the type of visit Other, Limit R is used for claims having the type of visit Referral and Limit E is used for claims having the type of visit Emergency.

    * ``Origin``

      It indicates where the price for remuneration of the item, comes from: This may be adjusted per medical item, the options are: [P] Price taken from the price list of a claiming health facility, [O] Price taken from a claim and [R] Relative price, the nominal value of which is taken from the price list and the actual value of which is determined backwards according to available funds and the volume of claimed services and medical items in a period. [R] is the default value.

    * ``Adult``

      It indicates the limitation for adults. If the type of limitation is a co-insurance then the value is the percentage of the price covered for adults by policies of the insurance product. If the type of limitation is a fixed limit the value is an amount up to which price of the item is covered for adults by policies of the insurance product. Default is 100%. Adult O is for Other, Adult R is for Referral and Adult E is for Emergency claims according to the type of visit (Visit Type).

    * ``Child``

      It indicates the limitation for children. If the type of limitation is a co-insurance then the value is the percentage of the price covered for children by policies of the insurance product. If the type of limitation is a fixed limit the value is an amount up to which price of the service is covered for children by policies of the insurance product. Default is 100%. Child O is for Other, Child R is for Referral and Child E is for Emergency claims according to the type of visit (Visit Type).

    * ``No Adult``

      It indicates the maximal number of provisions of the medical item during the insurance period for an adult.

    * ``No Child``

      It indicates the maximal number of provisions of the medical item during the insurance period for a child.

    * ``Waiting Period Adult``

      It indicates waiting period in months (after the effective date of a policy) for an adult.

    * ``Waiting Period Child``

      It indicates waiting period in months (after effective date of a policy) for a child.

    * ``Ceiling Adult``

      It indicates whether the medical item is excluded from comparison against ceilings defined for adults in the insurance product. The default is that the medical item is not excluded from comparisons with ceilings. [H] means exclusion only for provision of in-patient care, [N] means exclusion only for out-patient care and [B] means exclusion both for in-patient and out-patient care.

    * ``Ceiling Child``

      It indicates whether the medical item is excluded from comparison against ceilings defined for children in the insurance product. The default is that the medical item is not excluded from comparisons with ceilings. [H] means exclusion only for provision of in-patient care, [N] means exclusion only for out-patient care and [B] means exclusion both for in-patient and out-patient care.

    * ``Account Code Remuneration``

      Enter the account code of the insurance product used in the accounting software for remuneration of the product. 25 characters maximum.

    * ``Account Code Contribution``

      Enter the account code of the insurance product used in the accounting software for paid contributions. 25 characters maximum.

    * ``Registration Lump Sum``

      Enter the lump sum (for a household/group) for registration fee to be paid at the first enrolment of the household/group. Registration fee is not paid for renewals of policies.

    * ``Assembly Lump Sum``

      Enter the lump sum (for a household/group) for additional assembly fee to be paid both at the first enrolment and renewals of policies.

    * ``Registration Fee``

      Enter the registration fee per member of a household/group. If registration lump sum is non zero, registration fee is not considered. Registration fee is not paid for renewals of policies.

    * ``Assembly Fee``

      Enter the assembly fee per member of a household/group. If assembly lump sum is non zero, assembly fee is not considered. Assembly fee is paid both at the first enrolment and renewals of policies.

    * ``Start Cycle 1``

    * ``Start Cycle 2``

    * ``Start Cycle 3``

    * ``Start Cycle 4``

      If one or more starting dates (a day and a month) of a cycle are specified then the insurance product is considered as the insurance product with fixed enrolment dates. In this case, activation of underwritten and renewed policies is accomplished always on fixed dates during a year. Maximum four cycle dates can be specified.

    * ``Ceiling Interpretation``

      Specify whether Hospital and Non-Hospital care should be determined according to the type of health facility (select [Hospital]) that provided health care or according to the type of health care (select [In-patient]) acquired from a claim. In the first case all health care provided in hospitals (defined in the field ``HF Level`` in the register of Health Facilities) is accounted for ``Hospital Ceilings/Deductibles`` and for calculation of relative prices for the ``Hospital`` part. It means that if clamed health care was provided out-patient in a hospital, it is considered for calculation of ceilings/deductibles and for calculation of relative prices as hospital care. In the second case only in-patient care (determined from a claim when a patient spent at least one night in a health facility) is accounted for ``Hospital Ceilings/Deductibles`` and for calculation of relative prices for hospital part. Other health care including out-patient care provided in hospitals is accounted for ``Non hospital Ceilings/Deductibles`` and also such health care is used for calculation of relative prices for non-hospital part. Mandatory.

    * ``Treatment``

      Deductibles and Ceilings for treatments may be entered for general care (``Hospitals and Non-hospitals``) or for hospital care (``Hospitals``) only and/or for non-hospital care (``Non-Hospitals``) only. An amount may be set, indicating the value that a patient should cover within his/her own means, before a policy of the insurance product comes into effect (``Deductibles``) or the ceiling (maximum amount covered) within a policy of the insurance product (``Ceilings``) for a treatment (the treatment is identified health care claimed in one claim)

    * ``Insuree``

      Deductibles and Ceilings for an insuree may be entered for general care (``Hospitals and Non-hospitals``) or for hospital care (Hospitals) only and/or for non-hospital care (``Non-Hospitals``) only. An amount may be set, indicating the value that an insuree should cover within his/her own means, before a policy of the insurance product comes into effect (``Deductibles``) or the ceiling (maximum amount covered) within a policy of the insurance product (``Ceilings``) for an insuree for the whole insurance period.

    * ``Policy``

      Deductibles and Ceilings for a policy may be entered for general care (``Hospitals and Non-hospitals``) or for hospital care (``Hospitals``) only and/or for non-hospital care (Non-Hospitals) only. An amount may be set, indicating the value that policy holders should cover within their own means, before a policy of the insurance product comes into effect (``Deductibles``) or the ceiling (maximum amount covered) for the policy (all members of a family/group) of the insurance product (``Ceilings``) for the whole insurance period.

    * ``Extra Member Ceiling``

      Additional (extra) ceiling for a policy may be entered for general care (``Hospitals`` and ``Non-hospitals``) or for hospital care (``Hospitals``) only and/or for non-hospital care (``Non-Hospital`` s ) only per a member of a family/group above ``Threshold Members``.

    * ``Maximum Ceiling``

      Maximal ceiling for a policy may be entered for general care (``Hospitals`` and ``Non-hospitals``) or for hospital care (``Hospitals``) only and/or for non-hospital care (``Non-Hospitals``) only if extra ceilings are applied for members of a family/group above ``Threshold Members``.

    * ``Number``

      Maximal number of covered claims per an insuree during the whole insurance period according to the category of a claim. The options are claims of the category ``Consultations``, ``Surgery``, ``Delivery`` and ``Antenatal care``. Maximal numbers may be also specified for Hospitalizations (in-patient stays) and (out-patient visits) ``Visits``. The claim category is determined as follows:

    +-----------------------------------------------------------------------+
    | If at least one service of the category *Surgery* is given in the     |
    | claim it is of category *Surgery*                                     |
    |                                                                       |
    | otherwise                                                             |
    |                                                                       |
    | if at least one service of the category *Delivery* is given in the    |
    | claim it is of category *Delivery*                                    |
    |                                                                       |
    | otherwise                                                             |
    |                                                                       |
    | if at least one service of the category *Antenatal care* is given in  |
    | the claim it is of category *Antenatal care*                          |
    |                                                                       |
    | otherwise                                                             |
    |                                                                       |
    | if the claim is a hospital one the claim it is of category            |
    | *Hospitalization*                                                     |
    |                                                                       |
    | otherwise                                                             |
    |                                                                       |
    | if at least one service of the category *Consultation* is given in    |
    | the claim it is of category *Consultation*                            |
    |                                                                       |
    | otherwise                                                             |
    |                                                                       |
    | the claim is of the category *Visit*                                  |
    +-----------------------------------------------------------------------+

    * ``Ceiling``

      Maximal amount of coverage can be specified for claims according to the category of a claim. The options are claims of the category ``Consultations``, ``Surgery``, ``Delivery``, ``Antenatal care``, Hospitalizations, and ``Visits``. The category of claim is determined according to the procedure described with ``Number``.

      `Note. It is possible to specify only one of the following ceilings –per Treatment, per Insuree or per Policy. If ceilings per category of claims are specified together with ceilings per Treatment, per Insuree or per Policy than evaluation of claims may be dependent under special circumstances on the order of claimed medical services/items in a claim.`

    * ``distribution Period``

      Distribution periods may be entered for general care (``Hospitals`` and ``Non-hospitals``), or for hospital care (``Hospitals``) only and/or for non-hospital care (``Non-Hospitals``) only. Select from the list (**NONE, Monthly, Quarterly, Yearly**), the period that is to be used for calculation of the actual value of relative prices for the insurance product; by clicking on the arrow on the right. The default value is ‘\ **NONE**\ ’ which means that relative prices are not calculated for general health care or for hospital care or non-hospital care within the insurance product. By selecting **Monthly, Quarterly** or **Yearly** will cause a pop-up (:ref:`Image 14<image14>`) with the relative periods (1 period for yearly, 4 for quarterly, 12 for monthly). Percentages should be entered to indicate the distribution over the periods as per the product description. Enter to each field an appropriate percentage of paid contributions for policies of the insurance product allocated proportionally to corresponding calendar period. It means, for example, that in case of the distribution **Monthly** we put in each slot percentage of paid contributions of the insurance product that are allocated to the corresponding month and that is to be used for calculation of relative prices.

      It is not required to enter a value in each period, zero values are accepted. Once all the percentage values have been entered, click on the button OK to submit the values to the respective grid. Clicking on the button ``Cancel`` will cancel the action closing the popup and cancelling the change in the distribution.

        .. _image14:
        .. |logo9| image:: /img/user_manual/image16.png
          :scale: 100%
        .. |logo10| image:: /img/user_manual/image17.png
          :scale: 100%
        .. |logo11| image:: /img/user_manual/image18.png
          :scale: 100%

        +-------+--------+--------+
        ||logo9|||logo10|||logo11||
        +-------+--------+--------+

          `Image 14 - Distribution Periods (Monthly – Quarterly – Yearly) - Product)`

    * ``Capitation Payment``

      The section allows definition of parameters of a capitation formula used for remuneration of selected levels of health facilities within the insurance product. The report `Capitation Payment` is used for calculation of the amount of capitation payment for individual health facilities. The parameters of the capitation formula are the following:

    * ``Level 1``

      The first level of health facilities can be selected that should be included in the calculation of capitation payments. The options are the following levels of a health facility: Dispensary, Health Centre, and Hospital.

    * ``Sub Level 1``

      The sub-level of the first level of health facilities can be selected that should be included in calculation of capitation payments. If the sub level is not selected, all health facilities of the specified level are included irrespective of their sub-level.

    * ``Level 2``

      The second level of health facilities can be selected that should be included in the calculation of capitation payments. The options are the following levels of a health facility: ``Dispensary``, ``Health Centre``, and ``Hospital``.

    * ``Sub Level 2``

      The sub-level of the second level of health facilities can be selected that should be included in calculation of capitation payments. If the sub level is not selected, all health facilities of the specified level are included irrespective of their sub-level.

    * ``Level 3``

      The third level of health facilities can be selected that should be included in the calculation of capitation payments. The options are the following levels of a health facility: ``Dispensary``, ``Health Centre``, and ``Hospital``.

    * ``Sub Level 3``

      The sub-level of the third level of health facilities can be selected that should be included in calculation of capitation payments. If the sub level is not selected, all health facilities of the specified level are included irrespective of their sub-level.

    * ``Level 4``

      The fourth level of health facilities can be selected that should be included in the calculation of capitation payments. The options are the following levels of a health facility: ``Dispensary``, ``Health Centre``, and ``Hospital``.

    * ``Sub Level 4``

      The sub-level of the fourth level of health facilities can be selected that should be included in calculation of capitation payments. If the sub level is not selected, all health facilities of the specified level are included irrespective of their sub-level.

    * ``Share of Contribution``

      The share of allocated contributions for given insurance product and the period specified for the report Capitation Payment that should be used for calculation of capitation payments for individual health facilities. The amount specified is interpreted as a percentage.

    * ``Weight of Population``

      The weight can be entered that is used for the number of population living in catchments areas of individual health facilities. The amount specified is interpreted as a percentage.

    * ``Weight of Number of Families``

      The weight can be entered that is used for the number of families living in catchments areas of individual health facilities. The amount specified is interpreted as a percentage.

    * ``Weight of Insured Population``

      The weight can be entered that is used for the number of insured population by given insurance product and living in catchments areas of individual health facilities. The amount specified is interpreted as a percentage.

    * ``Weight of Number of Insured Families``

      The weight can be entered that is used for the number of insured families by given insurance product and living in catchments areas of individual health facilities. The amount specified is interpreted as a percentage.

    * ``Weight of Number of Visits``

      The weight can be entered that is used for the number of contacts of insured by given insurance product and living in catchments areas of individual health facilities. The amount specified is interpreted as a percentage.

    * ``Weight of Adjusted Amount``

      The weight can be entered that is used for the adjusted amount on claims for insured by given insurance product and living in catchments areas of individual health facilities. The amount specified is interpreted as a percentage.

    *Note. The capitation formula is defined as follows:*

      .. math::`\text{CapitationPayment}_{i} = \sum_{a}^{\ }{(\ \text{Indicator}_{i}^{a}} \times \frac{AllocatedContribution \times ShareContribution \times \text{Share}^{a}}{\sum_{i}^{\ }{\text{In}\text{dicator}}_{i}^{a}})`

      *Where*

      :math:`\text{CapitationPayment}_{i}` *is the amount of capitation payment for i-th health facility*

      :math:`\text{Indicator}_{i}^{a}` *is the value of the indicator of the type a for the i-th health facility.* :math:`\text{Indicator}_{i}^{a}`

      *may be:*

        - *Population living in catchments area of the health facility*
        - *Number of families living in catchments area of the health facility*
        - *Insured population living in catchments area of the health facility*
        - *Insured number of families living in catchments area of the health facility*
        - *Number of claims (contacts) with the health facility by insured in the catchment area*
        - *Adjusted amount*\

      :math:`\text{AllocatedContribution}` *is the amount of contributions for given insurance product for given period*

      :math:`\text{ShareContribution}` *is the formula parameter Share of contribution*

      :math:`\text{Share}^{a}` *is the weight of the indicator of the type a .*

      :math:`\text{Share}^{a}` *may be:*

      - *Weight of Population*
      - *Weight of Number of Families*
      - *Weight of Insured Population*
      - *Weight of Number of Insured Families*
      - *Weight of Number of Visits*
      - *Weight of Adjusted Amount*

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Product Control Page <#product-control-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the product has been saved will appear on the Information Panel.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right of the corresponding data field).

 #. **Cancel**

    By clicking on the ``Cancel`` button, the user will be re-directed to the `Product Control Page <#product-control-page>`__.

Adding a Product
""""""""""""""""

  Click on the ``Add`` button to re-direct to the `Product Page <#claim-administrators-administration>`__\ .

  When the page opens all entry fields are empty. See the `Product Page <#claim-administrators-administration>`__ information on the data entry and mandatory fields.

Editing a Product
"""""""""""""""""

  Click on the ``Edit`` button to re-direct to the `ProductPage <#claim-administrators-administration>`__\ .

  The page will open with the current information loaded into the data entry fields. See the `Product Page <#claim-administrators-administration>`__ for information on the data entry and mandatory fields

Duplicating a Product
"""""""""""""""""""""

  Click on the ``Duplicate`` button to re-direct to the `Product Page <#claim-administrators-administration>`__\ .

  The page will open with all the current information for the selected product, (except for the product code which should be unique), loaded into the data entry fields. See the `Product Page <#claim-administrators-administration>`__ for information on the data entry and mandatory fields. To save the record, enter a unique code before clicking on save.

Deleting a Product
""""""""""""""""""

  Because of potential problems with synchronization of data between off-line and on-line version, it is not possible delete insurance products currently.
