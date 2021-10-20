Contract
^^^^^^^^

  The contract define the wished coverage for a given list of isuree for a defined period

Pre-conditions

  Contract works only with group insurance so far but this might evolve in the futur

Navigation

  All functionality for use with the administration of contract can be found under the main menu ``Insurees and Policies``, sub menu ``Contract``.

  .. _contract_menu:
  .. figure:: /img/user_manual/contract.menu.png
    :align: center

    `Navigation Contract`

  Clicking on the sub menu ``contract`` re-directs the current user to the Find contract Page.


  .. _contract_search:
  .. figure:: /img/user_manual/contract.search.png
    :align: center

    `Search Contract`


Search Page
+++++++++++

  1. Search criteria

    * Code: code of the policyholder, often given during the registration process

    * Policyholder: contract for a given policy holder

    * Amount from/to: serach contract by amount

    * Payment due date

    * Payment reference

    * Amendement: search for amendement (0 is none)

    * Date Valid from/to: Period covered by the contract

    * State: status of the contract

    * show deleted: show deleted policyhodler

  2. reset search criteria

  3. apply the search criteria

  4. Result pane

    the columns name definiction matches with the search criteria definitions

    the rows are the search results


  5. Edit policyholder

    as doubleclick on the line, clicking on that button will open the policyholder Page
    
  6. Delete policyhodler

    Confirmation pop up is displayed


  7. standard notification panel for async message (deletion / creation / updates ... )

Card
++++

    .. _contract_details:
    .. figure:: /img/user_manual/contract.details.png
      :align: center

      `Navigation Contract`

  General inforamation

    
    * Code: code of the contract

    * Policyholder: contract for the given policy holder

    * amounts

        * notified : the amount when the contract was created, based on insuree default calculation parameters

        * rectified: the amount after modification of the contract (add/remove insuree, change of the calculation params ..  )

        * Due: amount after validation of the schem admin

    * Date approved: date when the scheme admin approaved the contract

    * Payment due date

    * State: status of the contract

    * Payment reference

    * Amendement:  amendement number (0 is none)

    * Date Valid from/to: Period covered by the contract

  button

    The button in 10 is reject a contract, required the approve rights and the contract to be in "negociable" state

    The button in 11 is approve a contract, required the approve rights and the contract to be in "negociable" state

    The button submit a contract, required the submit rights and the contract to be in "draft" or "Counter" state

    .. _contract_submit:
    .. figure:: /img/user_manual/contract.submit.png
        :align: center

        `Search submit`
 
    The button submit a contract, required the amend rights and the contract to be in "effective" state

    .. _contract_amend:
    .. figure:: /img/user_manual/contract.amend.png
        :align: center

        `Search amend`

  contract details tab

    This tab shows the insuree linked to the contract

    Search

      * Insuree number

      * Contribution bundle plan

      Reset and aply search button are using the same icon as the PH

      "Create new Policy Holder Insuree" button will open a creation pop up

    Results

      see search part of the columns descriptions

      in addition to the standard column, the calcualtion column shows parameters that are pulled from the calcuation rules, in the picture the income is display in that column

      edit button will open a edit popup

      delete button will open a confirmation popup

      duplicate will open a creation popup



  Contribution plan tab

    this tab is used to link Contribution plan to policyholder in order to reduce the possible Contribution plan choice for the policyholders
    
    See contribution plan page for more details on contribution plan

  payement tab

    This tab shows the payments linked to policyholder contract

    See payment page for more details on payment

  person covered user

    this tab shows the persons covered by the contract it can the the insuree but also the dependant if the contribution plan foresee it

    see policyholder page




