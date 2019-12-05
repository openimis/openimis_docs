

Batch Run
^^^^^^^^^

  Administration of batches of claims is restricted to users with the system role of Accountant or with a role including an access to Claims/Claim/Batch.

Pre-conditions
""""""""""""""

  A claim has been already processed (:ref:`review_actions`).

Navigation
"""""""""""

  All functionality for use with the administration of processing of batches can be found under the main menu ``Claims``, sub menu ``Batch Run`` (:numref:`batch_run_menu`).

  .. _batch_run_menu:
  .. figure:: /img/user_manual/claim.menu_batchrun.png
    :align: center

    `Navigation Batch Run`

  Clicking on the sub menu ``Batch Run`` re-directs the current user to the `Batch Run Control Page <#batch-run-control-page>`__.

Batch Run Control Page
""""""""""""""""""""""

  .. _batch_run_page:
  .. figure:: /img/user_manual/claim.batch_run_page.png
    :align: center

    `Batch Run Control Page`

  The Batch Run Control Page is the central point for batch processing administration. Access to the page is restricted to users with the system role of Accountant or with a role including an access to Claims/Claim/Batch. By having access to this page, it is possible to process batches, filter, and filter for accounts. The panel is divided into six sections (:numref:`batch_run_page`)

 #. **Batch Processing Panel**  

    The batch processing panel allows a user to process batches based on the following criteria:

    * ``Region``

      Select the ``Region`` from the list of regions by clicking on the arrow on the right of the selector to select a region. *Note: The list will only be filled with the regions assigned to the current logged in user and the option National*.  The option ``National`` will process all the claim for the period specified in ``Month`` and ``Year``

    * ``District``

      Select the ``district`` from the list of districts by clicking on the arrow on the right of the selector to select a district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is the only one then the district will be automatically selected. If no district is selected then the processing is done only for insurance product defined for the selected region.*

    * ``Year``

      Select the ``Year`` from the list of available years by clicking on the arrow on the right of the selector. Only periods for which a batch hasn’t been run yet are offered in both lists.

    * ``Month``

      Select the ``Month`` from the list of months by clicking on the arrow on the right of the selector.

      The Month at the end of the quarter process the claim for insuree having a product with Quaterly distribution (:ref:`Product Page <product_distribution>`):

        * March     --> Process the claim for first quatrer

        * June      --> Process the claim for second quatrer

        * September --> Process the claim for Third quatrer

        * December  --> Process the claim for Fourth quatrer

      December process the claim for insuree having a product with Yearly distribution (:ref:`Product Page <product_distribution>`)


    * ``Process``

      Once criteria are chosen, clicking on this button (:numref:`batch_run_process`), the claims will be processed based on the selected criteria. If the option ``National`` was used in the field ``Region``, the batch will run only for nationwide insurance products. If a region is selected in the field ``Region`` and no district is selected, the batch will run only for regional insurance products for the selected region. If a district is selected in the field ``District`` the batch is run only for district insurance products for the selected district.

      .. _batch_run_process:
      .. figure:: /img/user_manual/mat.send.png
        :align: center

        `Batch Run Process Button`



 #. **Filter Panel for the relative price index per product and period**  

    The filter panel allows a user to filter the of indexes for relative pricing per period, product and zone (results of running of batches). In case the product doesn't have any distribution configured then no relative price index are calculated by running the batch meaning no record will be added to the below list.

    the Relative price indexes can be filtered based on the following criteria:

    * ``Type``

      Select the ``Type``; from the list of time group types (**Monthly, Quarterly, Yearly**) by clicking on the arrow on the right of the selector.

    * ``Year``

      Select the ``Year``; from the list of available years by clicking on the arrow on the right of the selector.

    * ``Period``

      Select the ``Period``; from the list of months/quarters by clicking on the arrow on the right of the selector.

    * ``Region``

      Select the ``Region``; from the list that appear after typing characters, all region containing the typed text will appear and be selectable underneath the box. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected*

    * ``District``

      Select the ``District``; from the list that appear after typing characters , all district containing the typed text will appear and be selectable underneath the box. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected*


    * ``Product``

      Select the ``Product``; from the list that appear after typing characters , all product containing the typed text will appear and be selectable underneath the box.

    * ``Category``

      Select category of health care (**In-patient/hospital, Out-patient/Non-hospital, All**) from the list of categories of health care by clicking on the arrow on the right of the selector.

    * ``Filter``

      Once criteria are chosen, clicking on this filter button (:numref:`batch_run_filter`) will filter based on the selection criteria.

      .. _batch_run_filter:
      .. figure:: /img/user_manual/mat.send.png
        :align: center

        `Batch Run filter Button`

 #. **Display Panel for the relative price index per product and period**

    The Display Panel is used to display results of running of batches after the filter or processing.

 #. **Filter for Accounts Panel**

    The Filter for Accounts Panel is used in filtering of batch protocols for an accounting system based on the following criteria:

    * ``Group By``

      Select either grouping of the report by health facility (``health facility``) or by product (``Product``).

    * ``Start Date``

      Type in a date; or use the Date Selector (:numref:`cal_picker`) to enter date which is equal or less than claim date. *Note. To clear the date entry box; use the ``Clear`` button on the date picker popup.*

    * ``End Date``

      Type in a date; or use the Date Selector (:numref:`cal_picker`) to enter date which is equal or greater than claim date. *Note. To clear the date entry box; use the ``Clear`` button on the date picker popup.*

    * ``Show Claims``

      Check this checkbox, if you need to show all claims in detailed way in the protocol.

    * ``Region``

      Select the ``Region``; from the list that appear after typing characters, all region containing the typed text will appear and be selectable underneath the box. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected*

    * ``District``

      Select the ``District``; from the list that appear after typing characters , all district containing the typed text will appear and be selectable underneath the box. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected*

    * ``Health facility``

      Select the ``Health facility``; from the list that appear after typing characters, all Health facility containing the typed text will appear and be selectable underneath the box.*Note: The list will only be filled with the Health facility belonging to the selected region and assigned to the current logged in user. If this is only one then the Health facility will be automatically selected*

    * ``Product``

      Select the ``Product``; from the list that appear after typing characters , all product containing the typed text will appear and be selectable underneath the box.

    * ``Health facility Level``

      Select a level from the list of levels of health facilities by clicking on the arrow on the right of the selector.

    * ``Show All``

      Check this checkbox, if you need to show all health facilities in the report although they have no claim included.

    * ``Preview``

      Once criteria are chosen, clicking on this preview button (:numref:`batch_run_print`) will create a protocol of the selected batch.

      .. _batch_run_print:
      .. figure:: /img/user_manual/mat.print.png
        :align: center

        `Accountant report preview Button`

 #. **Button Panel**

    This panel contains control button.

    * ``Back``

      By clicking on the back button (:numref:`mat_back`), the user will be re-directed to the :ref:`Home Page <home_page>`.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a batch has been processed, filtered or if there was an error at any time during the process of these actions.
