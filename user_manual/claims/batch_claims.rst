

Batch Run
^^^^^^^^^

  Administration of batches of claims is restricted to users with the system role of Accountant or with a role including an access to Claims/Claim/Batch.

Pre-conditions
""""""""""""""

Navigation
"""""""""""

  All functionality for use with the administration of processing of batches can be found under the main menu ``Claims``, sub menu ``Batch Run``.

  .. _image162:
  .. figure:: /img/user_manual/image133.png
    :align: center

    `Image 162 - Navigation Batch Run`

  Clicking on the sub menu ``Batch Run`` re-directs the current user to the `Batch Run Control Page <#batch-run-control-page>`__.

Batch Run Control Page
""""""""""""""""""""""

  .. _image163:
  .. figure:: /img/user_manual/image134.png
    :align: center

    `Image163 (Batch Run Control Page)`

  The Batch Run Control Page is the central point for batch processing administration. Access to the page is restricted to users with the system role of Accountant or with a role including an access to Claims/Claim/Batch. By having access to this page, it is possible to process batches, filter, and filter for accounts. The panel is divided into six sections  (:ref:`Image 163<image163>`)

 #. **Batch Processing Panel**  

    The batch processing panel allows a user to process batches based on the following criteria:

    * ``Region``

      Select the ``Region`` from the list of regions by clicking on the arrow on the right of the selector to select a region. *Note: The list will only be filled with the regions assigned to the current logged in user and the option National.*

    * ``District``

      Select the ``district`` from the list of districts by clicking on the arrow on the right of the selector to select a district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is the only one then the district will be automatically selected. If no district is selected then the processing is done only for insurance product defined for the selected region.*

    * ``Month``

      Select the ``Month`` from the list of months by clicking on the arrow on the right of the selector.

    * ``Year``

      Select the ``Year`` from the list of available years by clicking on the arrow on the right of the selector. Only periods for which a batch hasn’t been run yet are offered in both lists.

    * ``Process``

      Once criteria are chosen, clicking on this button, the claims will be processed based on the selected criteria. If the option ``National`` was used in the field ``Region``, the batch will run only for nationwide insurance products. If a region is selected in the field ``Region`` and no district is selected, the batch will run only for regional insurance products for the selected region. If a district is selected in the field ``District`` the batch is run only for district insurance products for the selected district.

 #. **Filter Panel**  

    The filter panel allows a user to filter results of running of batches (calculation of indexes for relative pricing) based on the following criteria:

    * ``Type``

      Select the ``Type``; from the list of time group types (**Monthly, Quarterly, Yearly**) by clicking on the arrow on the right of the selector.

    * ``Year``

      Select the ``Year``; from the list of available years by clicking on the arrow on the right of the selector.

    * ``Period``

      Select the ``Period``; from the list of months/quarters by clicking on the arrow on the right of the selector.

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select a region. *Note: The list will only be filled with the regions assigned to the current logged in user and the option National.*

    * ``District``

      Select the District; from the list of districts by clicking on the arrow on the right of the selector to select a district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected*

    * ``Product``

      Select Product from the list of products by clicking on the arrow on the right of the selector.

    * ``Category``

      Select category of health care (**Hospital, Non-hospital, General**) from the list of categories of health care by clicking on the arrow on the right of the selector.

    * ``Filter``

      Once criteria are chosen, clicking on this filter button will filter based on the selection criteria.

 #. **Display Panel**  

    The Display Panel is used to display results of running of batches after the filter or processing. While hovering over records, records get highlighted with a yellow colour (:ref:`Image 164<image164>`).

    .. _image164:
    .. figure:: /img/user_manual/image135.png
      :align: center

      `Image 164 - Selected record (blue), hovered records (yellow) - Result Panel`


 #. **Filter for Accounts Panel**  

    The Filter for Accounts Panel is used in filtering of batch protocols for an accounting system based on the following criteria:

    * ``Start Date``

      Type in a date; or use the Date Selector Button to enter date which is equal or less than claim date. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``End Date``

      Type in a date; or use the Date Selector Button to enter date which is equal or greater than claim date. *Note. To clear the date entry box; use the mouse to highlight the full date and then press the space key.*

    * ``Date Selector Button``

      Clicking on the ``Date Selector Button`` will pop-up an easy to use, calendar selector (:ref:`Image 16<image16>`); by default the calendar will show the current month, or the month of the currently selected date, with the current day highlighted.

        - At anytime during the use of the pop-up, the user can see the date of **today**.
        - Clicking on today will close the pop-up and display the today’s date in the corresponding date entry box.
        - Clicking on any day of the month will close the pop-up and display the date selected in the corresponding date entry box.
        - Clicking on the arrow to the left displays the previous month.
        - Clicking on the arrow on the right will displays the following month.
        - Clicking on the month will display all the months for the year.
        - Clicking on the year will display a year selector.

        .. _image165:
        .. |logo45| image:: /img/user_manual/image6.png
          :scale: 100%
          :align: middle
        .. |logo46| image:: /img/user_manual/image7.png
          :scale: 100%
          :align: middle
        .. |logo47| image:: /img/user_manual/image8.png
          :scale: 100%
          :align: middle

        +----------++----------++----------+
        | |logo45| || |logo46| || |logo47| |
        +----------++----------++----------+

          `Image 165 - Calendar Selector - Search Panel`

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select a region. *Note: The list will only be filled with the regions assigned to the current logged in user and the option National.*

    * ``District``

      Select the ``district``; from the list of districts by clicking on the arrow on the right of the selector to select a district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the District will be automatically selected*

    * ``HF``

      Select a health facility from the list of health facilities codes and names clicking on the arrow on the right of the selector. *Note: The list will only be filled with the Health Facilities belonging to the Districts assigned to the current logged in user.*

    * ``Product``

      Select a product from the list of products by clicking on the arrow on the right of the selector. The list of products contains only nationwide insurance products if the option **National** is used in the field Region. It contains only regional insurance products for the selected region if no district is selected. It contains only district insurance products for the selected district.

    * ``Level``

      Select a level from the list of levels of health facilities by clicking on the arrow on the right of the selector.

    * ``Group By``

      Select either grouping of the report by health facility (``HF``) or by product (``Product``) by checking either the health facility checkbox or product checkbox respectively.

    * ``Show All``

      Check this checkbox, if you need to show all health facilities in the report although they have no claim included.

    * ``Show Claims``

      Check this checkbox, if you need to show all claims in detailed way in the protocol.

    * ``Preview``

      Once criteria are chosen, clicking on this preview button will create a protocol of the selected batch.

 #. **Button Panel**

    This panel contains control button.

    * ``Cancel``

      By clicking on the cancel button, the user will be re-directed to the `Home Page <#image-2.2-home-page>`__.

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a batch has been processed, filtered or if there was an error at any time during the process of these actions.
