Invoices
^^^^^^^^^^^^

Pre-conditions
==============
In order to create an invoice a family must be enrolled. Navigate to the ``Families/Groups`` under ``Insurees and Policies`` menu and find the family you wish to create an invoice for.

Ones the family is located create a new policy. In order to know how to create a new policy head over to the :doc:`policy` page. 

Navigation
==========
Ones the policy is created navigate to the ``Invoices`` under ``Legal and Finance`` menu

.. _invoice_menu:
.. figure:: /img/user_manual/invoices.menu.png
    :align: center


Newly created invoice can be found here. 

.. _invoice_list:
.. figure:: /img/user_manual/invoices.list.png
    :align: center



The ``Invoices`` is the first step in the process of finding an invoice and thereafter accessing an invoice. This initial page nca be used to search for specific invoices based on specific criteria. The panel is divided into two main panels. 

Search Panel
""""""""""""""""
The Search Panel allows a user to select specific criteria to minimise the search result. In the case of invoices the following search options are available which can be used alone or in combination with eath other. 

Subject
    Select the ``Subject``; from the list of subjects by clicking on the arrow on the right of the sector to select invoices from a specific subject.

    Invoices can be filtered by the following subjects
        -  **Contract** (Invoices created for contracts)
        -   **Family** (Invoices created for families by creating policies)

Recipient
    Select the ``Recipient``; from the list of recipients by clicking on the arrow on the right of the sector to select invoices from a specific recipient. 

    Invoices can be filtered by the following recipients
        - **Insuree** (Invoice for a specific insuree)
        - **Policy Holder** (Invoice for a specific organization)

Code 
    Enter the ``Code`` of the either Insuree or Policy Holder depending on the Recipient to select invoices for a specific code.

Date Invoice
    Use the :ref:`date selector <cal_picker>` to enter the ``Date Invoice`` to search for invoices with an ``Invoice Date`` equal or earlier than the specified date.

Status
    Select the ``Status``; from the list of statuses by clicking on the arrow on the right of the sector to select invoices from a specific subject.

    An invoice can have the following statuses
        - **Draft**
        - **Validated** (When the invoice is generated)
        - **Paid** (When the invoice is fully paid)
        - **Canceled** (When the invoice is canceled)
        - **Deleted** (When the invoice is deleted from the system)
        - **Suspended**

Amount Total
    Type in a positive ``Invoice Amount`` to search for invoices with a total amount equal or greater than the typed amount. For example if 1000 is entered, then only invoices with an amount equal or greater than 1,000 will be displayed.

Result Panel
"""""""""""""

The result panel displays a list of all invoices found matching the selected criteria in the search panel. The current selected record is highlighted. On the right side of the row you can find all the actions available. You can also double click on an invoice to view the invoice deatils.


.. _invoice_result_panel:
.. figure:: /img/user_manual/invoice.resultpanel.png
    :align: center

    `Edit invoice, Delete invoice`

Invoice Page
"""""""""""""
.. _invoice_page:
.. figure:: /img/user_manual/invoice.page.png
    :align: center

    `Invoice detail`

General information
-------------------
General information about the selected invoice

Line Items
-----------
.. _invoice_line_items:
.. figure:: /img/user_manual/invoice.lineitems.png
    :align: center

    `Items in the invoice`

Search criteria
""""""""""""""""
List of the items in an invoice can be filtered by search criteria panel. Here are the possible search parameters. The result of the search can be seen in the panel below.

Code
    Enter the item code to filter the items by code

Description
    Enter the full description or a part of the description to filter the item list

Ledge Account
    Enter the full or part of the ledger account to filter the item list

Quantity
    Enter the quantity to filter the item list by quantity

Unit Price
    Enter the unit price to filter the item list by unit price

Discount
    Enter the discount amount to filter the item list by discount

Deduction
    Enter the deduction amount to filter the item list by deduction amount

Amount Total
    Enter the total amount to filter the item list by amount

Amount next
    Enter the net amount to filter the list by net amount


Payments
-------------

.. _invoice_payment:
.. figure:: /img/user_manual/invoice.payments.png
    :align: center

    `Payments for the selected invoice`

Search criteria
""""""""""""""""
List of the payments for the selected invoice can be filtered by search criteria panel. Here are the possible search parameters. The result of the search can be seen in the panel below.

Reconciliation Status

.. _invoice_recon_filter:
.. figure:: /img/user_manual/invoice.reconcile_filter.png
    :align: center

    `Reconciliation status filter`


Select the reconciliation status of the payments to filter the payment. Following are the possible statuses.

    - **Not reconciliated** (The payment has not been reconciliated yet)
    - **Reconciliated** (The payment has been reconciliated in the system)
    - **Refunded** (The payment has beed refunded)
    - **Cancelled** (The payment has been cancelled)

Code
    Enter the payment  code to filter the payment list

Label
    Enter the label to filter the payment list by label text

Code Thirdparty
    Enter the Code thirdparty to filter the payment list by third party code text

Receipt number
    Enter the receipt number to filer the payment list by the receipt number

Fees
    Enter the fees amount to filter the payment list by fees amount

Amount Receieved
    Enter the amount receieved to filter the payment liset by received amount

Payment Date
    Use the :ref:`date selector <cal_picker>` to enter the ``Payment Date`` to search for payments with a ``Payment Date`` equal or earlier than the specified date.

Payment origin
    Enter the payment origin to filter the payment list by the origin of the payment

Payer Reference
    Enter the payer reference to filter the payment list by payer


Create new Payment
==================

To enter a new payment for the selected invoice. Click on the Add (+) icon

.. _invoice_payment_new:
.. figure:: /img/user_manual/mat.add.png
    :align: center


This will open up the following form to enter the payment detail

.. _invoice_new_payment:
.. figure:: /img/user_manual/invoice.new_payment.png
    :align: center

    `New payment`

Reconciliation Status
    Select the reconciliation status of the payment. Mandatory.
    Different types of statuses can be found :ref:`here <invoice_recon_filter>`

Status:
    Select the status of the payment. Mandatory. Following are the possible status of the payment

    - **Rejected** (The payment is rejected)
    - **Accepted** (The payment is accepted)
    - **Refunded** (This is the refund)
    - **Cancelled** (The payment has been cancelled)

Payer Reference
    Enter the payment reference. Mandatory

Payer Name
    Enter the name of the payer. Mandatory

Code
    Enter the unique payment code. Mandatory

Label
    Enter the label text for the payment. Mandatory

Code Thirdparty
    Enter the third party code for the payment. Mandatory

Receipt number
    Enter the unique receipt number for the payment. Mandatory

Fees
    Enter the fees amount for the payment. Mandatory

Amount received
    Enter the amount received. Mandatory

Payment Date
    Use the :ref:`date selector <cal_picker>` to enter the ``Payment Date``. Mandatory

Payment origin
    Enter the origin of the payment. Mandatory

Ones all the details are filled out, click on the ``CREATE`` button to create a new payment for the selected invoice. User can click on the ``CANCEL`` button to cancel the operation.

.. _invoice_new_payment_list:
.. figure:: /img/user_manual/invoice.new_payment_list.png
    :align: center

    `Payment List`

Ones a new payment is created successfully, it can be found under the ``Payments`` tab. The payment can be deleted by clicking on the trash icon from the right side of the list. Ones the user click on the trash icon, they will be prompted by a confirmation dialog. The payment will be either deleted or the operation will be cancelled depending on the action selected from the confirmation dialog.

.. _invoice_delete_payment:
.. figure:: /img/user_manual/invoice.delete_payment.png
    :align: center

    `Confirmation dialog to delete the payment`




