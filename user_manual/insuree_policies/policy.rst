Policy
^^^^^^

.. contents:: Table of Contents

Find Policy
===========

Access to the ``Find Policy Page`` is restricted to users with the role system roles of Accountant, Clerk or Health Facility Receptionist or with a role including an access to Insurees and Families/Policy/Search.

Pre-conditions
--------------

Need to enquire on, or edit a policy, and the family/group, insurees and contributions associated.

Navigation
----------

Find Policy Page can be found under the main menu ``Insurees and Policies``, sub menu ``Policies``.

.. _image101:
.. figure:: /img/user_manual/image79.png
  :align: center

  `Navigation Policies`

Clicking on the sub menu ``Policies`` re-directs the current user to the ``find policy page.``

Page
----

  .. _image102:
  .. figure:: /img/user_manual/80_policies_find.png
    :align: center

  `Find Policy Page`

  The ``Find Policy Page`` is the first step in the process of finding a policy and thereafter accessing the
  `Family Overview Page <#family-overview-page.>`__ of insurees, policies and contributions. This initial page can be
  used to search for specific policies or groups of policies based on specific criteria. The panel is divided into two
  main panels (:numref:`image102`)

 #. **Search Panel**

    The Search Panel allows a user to select specific criteria to minimise the search results.
    In the case of policies the following search options are available which can be used alone or in combination with each other.

    * ``Region``

      Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select policies from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected.*

    * ``District``

      Select the ``District``; from the list of districts by clicking on the arrow on the right of the selector to select policies for families/groups residing in a specific district. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user. If this is only one then the district will be automatically selected.*

    * ``Product``

      Select the ``Product``; from the list of products by clicking on the arrow on the right of the selector, to select policies for a specific product.

    * ``Enrolment Officer``

      Select the ``Enrolment Officer``; from the list of enrolment officers by clicking on the arrow on the right of the selector, to select policies related to a specific enrolment officer.

    * ``Enrolment Date From``

      Use the :ref:`date selector <cal_picker>` to enter the ``Enrolment Date From`` to search for policies with an ``Enrolment Date`` equal or later than the specified date.

    * ``Enrolment Date To``

      Use the :ref:`date selector <cal_picker>` to enter the ``Enrolment Date to`` to search for policies with an ``Enrolment Date`` equal or earlier than the specified date.

    * ``Start Date From``

      Use the :ref:`date selector <cal_picker>` to enter the ``Start Date From`` to search for policies with a ``Start Date`` equal or later than the specified date.

    * ``Start Date To``

      Use the :ref:`date selector <cal_picker>` to enter the ``Start Date to`` to search for policies with a ``Start Date`` equal or earlier than the specified date.

    * ``Effective Date From``

      Use the :ref:`date selector <cal_picker>` to enter the ``Effective Date From`` to search for policies with an ``Effective Date`` equal or later than the specified date.

    * ``Effective Date To``

      Use the :ref:`date selector <cal_picker>` to enter the ``Effective Date To`` to search for policies with an ``Effective Date To`` equal or earlier than the specified date.

    * ``Expiry Date From``

      Use the :ref:`date selector <cal_picker>` to enter the ``Expiry Date From`` to search for policies with an ``Expiry Date`` equal or later then the specified date.

    * ``Expiry Date To``

      Use the :ref:`date selector <cal_picker>` to enter the ``Expiry Date To`` to search for policies with an ``Expiry Date`` equal or earlier then the specified date.

    .. include:: ../date_picker.rst

    * ``Policy Type``

      Select whether new policies [New Policy] or renewed policies [Renewal] should be searched for.

    * ``Policy Status``

      Select the ``Policy Status``; from the list of policy statuses by clicking on the arrow on the right of the selector, to select policies for a specific policy status.

      A policy can have the following statuses:

        - **Idle** (Policy data entered but policy not yet activated)
        - **Active** (Policy partially or fully paid and made active)
        - **Suspended** (Policy was not fully paid for within the grace period)
        - **Expired** (Policy is not active anymore as the insurance period elapsed)

    * ``Balance``

      Types in a positive ``Balance`` to search for policies with a balance equal or greater than the typed amount. For example if 0 (zero) is entered, all policies with a balance, will be displayed. If 1,000 is entered, then only policies with a balance equal to or greater than 1,000 will be displayed.

      The balance is the difference between the policy value and total of contributions paid. For the policy

    * ``Only with inactive insurees``

      Check the box to select only policies for families/groups with insurees which are non-active (not covered) despite the policy of their family/group is active. The reason may be addition of a new insuree (member) to the family/group with an active policy without adequate payment of additional contributions or because the maximum number of members in the family/group exceeds the maximum number determined by the insurance product of the policy.

    * ``Show historical``

      Click on ``Historical`` to see historical records matching the selected criteria. Historical records are displayed in grey to define them from current records (:numref:`image104`) and do not have action buttons.

      .. _image104:
      .. figure:: /img/user_manual/81_policies_historical.png
        :align: center

        `Historical records - Result Panel`


 #. **Result Panel**

    The Result Panel displays a list of all policies found, matching the selected criteria in the search panel. The currently selected record is highlighted (:numref:`image105`). On the right are the available action buttons. One can also double-click on the row to view the policy details.

    .. _image105:
    .. figure:: /img/user_manual/82_policies_actions.png
      :align: center

      `Open family, Open in new tab, Renew policy, Suspend policy, Delete policy`


Policy Page
"""""""""""

  .. _image128:
  .. figure:: /img/user_manual/102_policies_view.png
    :align: center

    `Policy Page`


 #. **Family Details**

    Summary of the family concerned by this policy

 #. **Policy Details**

    * ``Enrolment Date``

      Enter the enrolment date for the policy. Mandatory. *Note: You can also use the button next to the enrolment date field to select a date to be entered.*

    * ``Effective Date``

      The effective date for the policy is calculated automatically later on. The effective date is the maximum of the start date and the date when the last contribution was paid or when the user enforced activation of the policy.

    * ``Start Date``

      The start date for the policy is calculated automatically. Either it is the enrolment date plus the administration period of the insurance product associated with the policy for free enrolment (without cycles) or it is a cycle start date determined according to enrolment date and the administration period for enrolment in fixed cycles. The start date may be modified by the user.

    * ``Expiry Date``

      The expiry date for the policy is calculated automatically. When entering a new policy, the expiry date is the start date plus the insurance period of the insurance product associated with the policy for free enrolment or the cycle start date plus the insurance period for enrolment in fixed cycles.

    * ``Product``

      Select from the list of available products the product of the policy. Mandatory.

    * ``Enrolment Officer``

      Select from the list of available enrolment officers the enrolment officer related to the policy. Mandatory

 #. **Policy Values**

    * ``Value``
    * ``Contributions paid``
    * ``Balance``
    * ``Deductible``

      Deductible amounts for the categories: General, In-Patient and Out-Patient

    * ``Remunerated Health Care``

      Remunerated amounts for the categories: General, In-Patient and Out-Patient


 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Family Overview Page, <#family-overview-page.>`__ with the newly saved record displayed and selected in the result panel.


Adding a Policy
"""""""""""""""

  To create a new policy for a family that doesn't have any yet, head over to the :ref:`Family Page <family_overview_page>` and in the policies section, use the plus sign on the top right.

  .. _image128b:
  .. figure:: /img/user_manual/family_policies.png
    :align: center

    `Policies section of the Families page`

Renewing a Policy
"""""""""""""""""

  Click on the ``renewal arrows`` to go to the `Policy Page <#policy-page>`__\ .

Region
  Select the ``Region``; from the list of regions by clicking on the arrow on the right of the selector to select policies from a specific region. *Note: The list will only be filled with the regions assigned to the current logged in user. If this is only one then the region will be automatically selected.*

Pausing a Policy
""""""""""""""""

  Click on the ``pause symbol`` to get a confirmation dialog and pause the corresponding policy.

  .. _image129p:
  .. figure:: /img/user_manual/policies_suspend_confirmation.png
    :align: center

    `Pause policy - confirmation`


Deleting a Policy
"""""""""""""""""

  Click on the ``trashcan icon`` to delete the currently selected policy.

  Before deleting of a policy, all contributions of the policy should be deleted. Before deleting a confirmation popup (:numref:`img_policies_delete_confirmation`) is displayed, which requires the user to confirm if the action should really be carried out.

  .. _img_policies_delete_confirmation:
  .. figure:: /img/user_manual/policies_delete_confirmation.png
    :align: center

    `Historical records - Result Panel`


Result Panel
"""""""""""""

The Result Panel displays a list of all policies found, matching the selected criteria in the search panel. The currently selected record is highlighted (:numref:`image105`). On the right are the available action buttons. One can also double-click on the row to view the policy details.

.. _image105:
.. figure:: /img/user_manual/82_policies_actions.png
  :align: center

  `Open family, Open in new tab, Renew policy, Suspend policy, Delete policy`


Policy Page
============

  .. _image128:
  .. figure:: /img/user_manual/102_policies_view.png
    :align: center

    `Policy Page`


Family Details
--------------

Summary of the family concerned by this policy.

Policy Details
--------------

Enrolment Date
  Enter the enrolment date for the policy. Mandatory. *Note: You can also use the button next to the enrolment date field to select a date to be entered.*

Effective Date
  The effective date for the policy is calculated automatically later on. The effective date is the maximum of the start date and the date when the last contribution was paid or when the user enforced activation of the policy.

Start Date
  The start date for the policy is calculated automatically. Either it is the enrolment date plus the administration period of the insurance product associated with the policy for free enrolment (without cycles) or it is a cycle start date determined according to enrolment date and the administration period for enrolment in fixed cycles. The start date may be modified by the user.

Expiry Date
  The expiry date for the policy is calculated automatically. When entering a new policy, the expiry date is the start date plus the insurance period of the insurance product associated with the policy for free enrolment or the cycle start date plus the insurance period for enrolment in fixed cycles.

Product
  Select from the list of available products the product of the policy. Mandatory.

Enrolment Officer
  Select from the list of available enrolment officers the enrolment officer related to the policy. Mandatory

Policy Values
-------------

Value
  Value

Contributions paid
  Amount of contribution paid

Balance
  Balance

Deductible
  Deductible amounts for the categories: General, In-Patient and Out-Patient

Remunerated Health Care
  Remunerated amounts for the categories: General, In-Patient and Out-Patient


Saving
------

Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Family Overview Page, <#family-overview-page.>`__ with the newly saved record displayed and selected in the result panel.


Adding a Policy
===============

To create a new policy for a family that doesn't have any yet, head over to the :ref:`Family Page <family_overview_page>` and in the policies section, use the plus sign on the top right.

.. _image128b:
.. figure:: /img/user_manual/family_policies.png
  :align: center

  `Policies section of the Families page`

Renewing a Policy
=================

Click on the ``renewal arrows`` to go to the `Policy Page <#policy-page>`__\ .

The page will open with the current information loaded into the data entry fields. See the `Policy Page <#policy-page>`__ for information on the data entry and mandatory fields.

Pausing a Policy
================

Click on the ``pause symbol`` to get a confirmation dialog and pause the corresponding policy.

.. _image129p:
.. figure:: /img/user_manual/policies_suspend_confirmation.png
  :align: center

  `Pause policy - confirmation`


Deleting a Policy
=================

Click on the ``trashcan icon`` to delete the currently selected policy.

Before deleting of a policy, all contributions of the policy should be deleted. Before deleting a confirmation popup (:numref:`img_policies_delete_confirmation`) is displayed, which requires the user to confirm if the action should really be carried out.

.. _img_policies_delete_confirmation:
.. figure:: /img/user_manual/policies_delete_confirmation.png
  :align: center

  `Delete confirmation- Button Panel`

When a policy is deleted, all records retaining to the deleted policy will still be available by selecting historical records.

