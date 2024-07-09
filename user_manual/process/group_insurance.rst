Group insurance
^^^^^^^^^^^^^^^

openIMIS is supporting group insurance since the October 2021 release, this feature allows a "policyholder" to take insurance for other insuree.

This feature does not change the insuree registration process, therefore the insuree must be already known by openIMIS before being attached to a policyholder.


Getting started
===============

openIMIS must have those configured:

 - Products

 - Locations

 - Health Facilities

Before starting the configuration of openimis the scheme must be defined upfront

this features don't covers the registration of the insuree, insuree must be registered using other openIMIS functions



#. Setting up the contribution plans

    This feature comes with contribution plans, those items are used to bring flexibility in the pricing models for a product. thanks to contributions plan, the scheme administrator can define different pricing for the same coverage.

    Before setting up the policyholder the scheme administrator must setup the contribution plans and then make bundle of contribution plan; even if only one contribution plan (product) is wished to be available for group insurance on "bundle" must still be created.

#. Creating the policyholder

    Once the general information regarding the Policyholder is saved, the eligible contribution plan bundle for that policyholder must be linked in the "contribution plan bundle" tab.

#. add Policyholder users

    to allow the inputs from the policyHolder, openimis user can be configure to the PH user, so they will have access the data that need to be maintained by the policyholders

#. Adding insuree on the policyholder

    Insuree can be added via the "policyholder insuree" tab, the clerk will have to find the insuree using the insuree number, then the policyholder contribution bundle plan (PH-CBP) need to be attached to the insuree

    Once PH-CBP is selected, the calculation params will be pulled (eg. invoice) and new inputs fields might apprears

#. Generating coverage

    Used to generate coverage the group insurance features used contracts.

    At creation the contrat will pull the valid PH-Insuree, once created (draft), the contract will have to go through severals steps : submitted (negociable) , approved (executable) , payed (Effective) then the coverage are active for the contract dates (can be modulated by the contribution plans)

#. Generating payment to third parites

    Once a claim is approved a payment is likely to be due, if order to generate the appropriate payment, payment plans need to be used


.. toctree::
   :maxdepth: 2
   :caption: Group insurance configuration

   ../register/contribution_plan.rst
   ../register/contribution_plan_bundle.rst
   ../insuree_policies/policyholder.rst
   ../register/policyholder_users.rst
   ../insuree_policies/contract.rst
   ../insuree_policies/payment_plans.rst

