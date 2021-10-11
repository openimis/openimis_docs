Group insurance
---------------


openIMIS is supporting group insurance since the October 2021 release, this feature allows a "PolicyHolder" to take insurance for other insuree


This feature does not change the insuree registration process, therefore the insuree must be already known by openIMIS before being attached to a policyholder.


Getting started
+++++++++++++++

openIMIS must have those configured:

 - Products
 
 - locaitons

#. Setting up the contribution plans

    this feature comes with contribution plans, those items are used to bring flexibility in the pricing models for a product. thanks to contributions plan, the scheme administrator can define different pricing for the same coverage.

    Before setting up the policy holder the scheme administrator must setup the contribution plans and then make bundle of contribution plan; even if only one contribution plan (product) is wished to be available for group insurance on "bundle" must still be created.

#. Creating the Policy holder

    Once the general information regarding the Policyholder is saved, the eligible contribution plan bundle for that policy holder must be linked in the "contribution plan bundle" tab.

#. Adding insuree on the policyholder

    insuree can be added via the "policyholder insuree" tab, the clerk will have to find the insuree using the insuree number, then the policyholder contribution bundle plan (PH-CBP) need to be attached to the insuree

    once PH-CBP is selected, the calucation params will be pulled (eg. invoice) and new inputs fields might apprears

#. generating coverage

    to generate coverage the group insurance features used contracts.

    at creation the contrat will pull the valid PH-Insuree, once created (draft), the contract will have to go through severals steps : submitted (negociable) , approved (executable) , payed (Effective) then the coverage are active for the contract dates (can be modulated by the contribution plans)

    