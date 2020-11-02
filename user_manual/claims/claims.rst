

Claims
------

The functionality under the menu ``Claims`` allows complete processing of claims from their entering into IMIS, modification, submission to processing, automatic checking of their correctness, reviewing of them by medical officers, their evaluating and preparation of report to an accounting system for their remuneration to contractual health facilities. Each claim can be consequently in several states. Once it is entered to openIMIS (either by the mobile phone application **Claim Management** or typed in and saved in IMIS) it goes to the status **Entered**. 


#. **claim entry and submission**

   When it is submitted and it successfully passes at least some automatic checks, the claim goes to the status **Checked**. If the claim doesn’t pass automatic checking it goes to the status **Rejected** and its processing ends. The claim in the status **Checked** may be reviewed from medical point of view and/or a feedback on it can be collected from the patient. 


#. **claim review: scrutinisation and feedback**

   Medical reviewing and feedback acquiring can be by-passed. Ones such (manual) scrutiny of the claim is at the end, the claim may be pushed to the status **Processed**. 


#. **claim valuation**

   In this status the claim is evaluated in nominal prices, taking into account all ceilings, deductibles and other cost sharing rules associated with insurance product or products covering claimed health care. If there is no medical service or medical item price of which a relative one according to the corresponding insurance product, the claim goes automatically to the status **Valuated**. 

   If there is at least one medical service or medical item with relative pricing, the claim goes to the status **Valuated** only after a batch for corresponding period is run. The batch for a period (month, quarter, year) finishes evaluation of relative prices on claims on one hand and summarizes all claims in the period for accounting system that is external to openIMIS (it is not a part of it). 


#. **claims values based on stage**

   Different values (prices) of a claim are associated with each stage of processing of claims. When a claim is entered the value of the claim based on nominal prices of claimed medical services/items is designated as **Claimed Value**. **Claimed Value** is associated with the state **Entered**. The value of the claim after automatic checking of claims during submission of the claim and after manual interventions of medical officers is designated as **Approved Value**. **Approved Value** is associated with the state **Checked**. The value of the claim after corrections based on all cost sharing rules of covering insurance products is designated as **Adjusted Value**. **Adjusted Value** is associated with the state **Processed**. The final value of the claim taking into account actual value of relative prices is designated as **Paid Value**. **Paid Value** is associated with the state **Valuated**.

.. toctree::
   :maxdepth: 3

   hf_claims
   review_claims
   batch_claims