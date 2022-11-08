Payment Plans
^^^^^^^^^^^^^^^^^^

Payment plans is responsible for generating bills. 

.. contents:: Table of Contents

Pre-conditions
==============
In order to create a payment plan there must be at least one product needs to be created. 

Navigation
==========
Ones a product is available navigate to the ``Payment Plans`` under ``Legal and Finance`` menu

.. _payment_plans_menu:
.. figure:: /img/user_manual/payment_plans.menu.png
    :align: center

    `Navigate to Payment plans menu`

All the existing payment plans can be found here.

.. payment_plans:
.. figure:: /img/user_manual/payment_plans.png
    :align: center

    `Payment plans`


Search Panel
""""""""""""""

Code
    Enter a code to filter the payment plans

Name
    Enter the full name or the part of the name to filter the payment plans

Calculation resultpanel
    Select a calculation rule by clicking on the righ arrow in the dropdown. Here are the possible choices.

    - **Payment: Fee for Service** (Payment plans for fee for service)
    - **Payment: Capitation** (Payment plans for capitation)
    - **Payment: Commission** (Payment plans for commission)
    - **Payment: Fees** (Payment plans for fees)
    - **Payment: Unconditional Cash Payment** (Payment plans for unconditional cash payment)

Benefit product
    Select a product from the dropdown list by clikcing on the right arrow.

Periodicity
    This field represents a number of months a payment plan needs to be executed.

Valid from
    Use the :ref:`date selector <cal_picker>` to enter the ``Valid from`` to search for payment plans with a ``Valid from`` date equal or later than the specified date.


Valid to
    Use the :ref:`date selector <cal_picker>` to enter the ``Valid to`` to search for payment plans with a ``Valid to`` date equal or earlier than the specified date.

Show Deleted
    By clicking this checkbox a user can list all the deleted payment plans along with the valid ones.


Create new Payment Plan
==================

To create a new payment plan click on the Add (+) icon in the bottom right of the page.

.. _invoice_payment_new:
.. figure:: /img/user_manual/mat.add.png
    :align: center


This will open up the following form to enter the payment plan deatils

.. _payment_plan_new:
.. figure:: /img/user_manual/payment_plans.new.png
    :align: center

    `Create a new payment plan`

Code
    Enter a unique code for the payment plan. Mandatory

Name
    Enter a name for the payment plan. Mandatory

Calculation Rule
    Select a calculation rule from the dropdown list by clicking on the arrow on the right hand side. Here are the possible choices. Mandatory

    - **Payment: Fee for Service** (Payment plans for fee for service)
    - **Payment: Capitation** (Payment plans for capitation)
    - **Payment: Commission** (Payment plans for commission)
    - **Payment: Fees** (Payment plans for fees)
    - **Payment: Unconditional Cash Payment** (Payment plans for unconditional cash payment)

Benefit Product
    Select a product from the dropdown list by clicking on the arrow on the right hand side. Mandatory

Periodicity
    Enter the periodicity in terms of months. This means how often do you want to generate bills for the payment plans. For instance, entering 1 will generate a bill every month. Mandatory

Valid from
    Use the :ref:`date selector <cal_picker>` to enter the ``Valid from``. This indicates from which date this payment plan comes in effect. Mandatory

Valid to
    Use the :ref:`date selector <cal_picker>` to enter the ``Valid to``. This indicates until which date this payment plan is valid.

Additional parameters
    Additional parameters change based on the calculation rule selected.

    - **Payment: Fee for Service**

    .. _payment_plans_feeforservice_additionalparams:
    .. figure:: /img/user_manual/payment_plans.feeforservice_additionalparams.png
        :align: center

        `Additional parameters for the Calculation rule Payment: Fee for Service`
    
    Claim Type
        Here you can select for which claims this payment plan is valid. The options are All, Hospital/In-patient and None-hospital/Out-patient
    
    Level 1
        Here a user can define the first level. Options are Hospital, Dispensary and Health center.

    Sublevel 1
        Here a user can define the first sublevel. Options are District and Region

    Level 2
        Here a user can define the second level. Options are Hospital, Dispensary and Health center.

    Sublevel 2
        Here a user can define the second sublevel. Options are District and Region

    Level 3
        Here a user can define the third level. Options are Hospital, Dispensary and Health center.

    Sublevel 3
        Here a user can define the third sublevel. Options are District and Region

    Level 4
        Here a user can define the fourth level. Options are Hospital, Dispensary and Health center.

    Sublevel 4
        Here a user can define the fourth sublevel. Options are District and Region

    - **Payment: Capitation**

    .. _payment_plan_capitation_additionalparams:
    .. figure:: /img/user_manual/payment_plans.capitation_additionalparams.png
        :align: center
        
        `Additional parameters for the Calculation rule Payment: Capitation`

    Claim Type
        Here you can select for which claims this payment plan is valid. The options are All, Hospital/In-patient and None-hospital/Out-patient
    
    Level 1
        Here a user can define the first level. Options are Hospital, Dispensary and Health center.

    Sublevel 1
        Here a user can define the first sublevel. Options are District and Region

    Level 2
        Here a user can define the second level. Options are Hospital, Dispensary and Health center.

    Sublevel 2
        Here a user can define the second sublevel. Options are District and Region

    Level 3
        Here a user can define the third level. Options are Hospital, Dispensary and Health center.

    Sublevel 3
        Here a user can define the third sublevel. Options are District and Region

    Level 4
        Here a user can define the fourth level. Options are Hospital, Dispensary and Health center.

    Sublevel 4
        Here a user can define the fourth sublevel. Options are District and Region

    Share Contribution
        Enter the valid integer from 0 to 100 to define the percentage (%) of the share of allocated contribution for given insurance product and the period specified. 

    Weight Population
        Enter the valid integer from 0 to 100 to define the percentage (%) of the number of population living in catchment area of the individual health facility.
    
    Weight number families
        Enter the valid integer from 0 to 100 to define the percentage (%) of the numebr of families living in the catchment area of the individual health facility. 

    Weight number insure population
        Enter the valid integer from 0 to 100 to define the percentage (%) of the numner of insured population by given insurance product and living in the catchment area of the individual health facility.

    Weight number insured families
        Enter the valid integer from 0 to 100 to define the percentage (%) of the numner of insured families by given insurance product and living in the catchment area of the individual health facility.

    Weight number visits
        Enter the valid integer from 0 to 100 to define the percentage (%) of the number of contacts of insured by given insurace product and living in the catchment area of the individual health facility. 

    Weight amount adjusted
        Enter the valid integer from 0 to 100 to define the percentage (%) of the adjusted amount on claims for insured by given insurance product and living in the catchment area of the individual health facility. 

    .. Note::
        The capitation formula is defined as follow:

        :math:`\text{CapitationPayment}_{i} = \sum_{a}^{\ }{(\ \text{Indicator}_{i}^{a}} \times \frac{AllocatedContribution \times ShareContribution \times \text{Share}^{a}}{\sum_{i}^{\ }{\text{In}\text{dicator}}_{i}^{a}})`

        **Where**

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

    - **Payment: Commission**

    .. _payment_plans_commission_additionalparams:
    .. figure:: /img/user_manual/payment_plans.commission_additionalparams.png
        :align: center

        `Additionl parameters for the Calculation rule Payment: Commission`

    Commission Rate(%)
        Enter the valid number to define the percentage to be paid.

    
    - **Payment: Fees**

    .. _payment_plans_fees_additionalparams:
    .. figure:: /img/user_manual/payment_plans.fees_additionalparams.png
        :align: center

        `Additional parameters for the Calculation rule Payment: Fees`


    Fee rate(%)
        This is the total percentage of the amount needs to be paid.

    Payment origin  
        Enter the name of the origin of the payment. For instance, if the name of the payment gateway is ABC then the value should be ABC in this field.

    
    - Payment: Unconditional cash payment

    .. _payment_plans_unconditional_additionalparams:
    .. figure:: /img/user_manual/payment_plans.unconditional_additionalparams.png
        :align: center

        `Additional paramters for the calculation rule Payment: Unconditional cash payment`

    Lumpsum to be paid
        Enter a valid number to be paid as a lumpsum amount

    Invoice label
        Enter the label of the invoice to which the lumpsum amount applies


    Ones all the the mandatory fields are entered, click on the ``SAVE`` button in the bottom right of the page. The user will be redirected to the Payment plans page with the newly created record displayed and selected in the result panel.


Result Panel
"""""""""""""
.. _payment_panel_result
.. figure:: /img/user_manual/payment_plans.result_panel.png
    :align: center

    `List of all the payment plans created in the system`


Here is the list of payment plans with 3 different actions. 

    - **Add new version**

        .. _payment_plan_new_version:
        .. figure:: /img/user_manual/payment_plan.new_version_menu.png
            :align: center

        Click on the new version menu icon on the payment plan you want to create a new version. This will open the selected payment plan in an edit mode. Make the necessary changes and click on the save button. This will create a new record in the system with the changes applied. A user will be redirected to the previous page and a new version of the payment plan will be displayed in the result panel. This will also inactive the previous record.

    - **Edit**

        .. _payment_plan_edit_menu:
        .. figure:: /img/user_manual/payment_plan.edit_menu.png
            :align: center


        
        Click on the pencil icon on the payment plan you want edit. This will open the selected payment plan in edit mode.

        .. _payment_plan_edit_mode:
        .. figure:: /img/user_manual/payment_plan.edit_mode.png
            :align: center

            `Payment plan in edit mode`

        A user can modify the payment plan and then click on the save button at the bottom right of the page to save the changes.


    - **Delete**

        .. _payment_plan_delete_menu:
        .. figure:: /img/user_manual/payment_plan.delete_menu.png
            :align: center

        Click on the trash icon on the payment plan you want to delete. This will open up a confirmation dialog. 

        .. _payment_plan_delete:
        .. figure:: /img/user_manual/payment_plan.delete.png
            :align: center

            `Payment plan delete confirmation dialog`

        Confirm the action by clicking on the ``OK`` button and this will delete the payment plan. A user can click on the ``CANCEL`` button to abort the operation.
