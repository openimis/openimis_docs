

Medical Item Price Lists
^^^^^^^^^^^^^^^^^^^^^^^^

Pricelists of medical items are tools for specification which medical items and at which prices can be invoiced by contractual health facilities to the scheme administration. Administration of pricelists of medical items is restricted to users with the system role of Scheme Administrator or with a role including an access to Administration/Pricelists-Medical Items.

.. contents:: Table of Contents

Pre-conditions
==============

A price list of medical items may only be added, after an agreement with a health facility or a group of health facilities on specific prices. Editing of the price list may occur only after an approval of the management of the scheme administration. Deletion of a price list of medical items normally will occur when a price list becomes obsolete.

Navigation
===========

All functionality for use with the administration of medical items price lists can be found under the main menu ``Administration``, sub menu ``Price Lists``, sub menu ``Medical Items Price Lists``.

.. figure:: /img/user_manual/image40.png
  :align: center

  `Navigation Price Lists Medical Items`

Clicking on the sub menu ``Medical Items`` re-directs the current user to the `Price List Medical Items Control Page <#price-list-medical-items-control-page>`__\ .

.. figure:: /img/user_manual/image41.png
  :align: center

  `Price List Medical Items Control Page`

Price List Medical Items Control Page
=======================================

The ``Price List Medical Items Control Page`` is the central point for all medical item price list administration. By having access to this panel, it is possible to add, edit, delete and search. The panel is divided into four panels (:numref:`image48`).

Search Panel
""""""""""""

The search panel allows a user to select specific criteria to minimise the search results. In the case of price lists for medical items the following search options are available which can be used alone or in combination with each other.

Name
  Type in the beginning of; or the full ``Name``; to search for price lists medical items with a Name, which starts with or matches completely, the typed text.

Date
  Type in the full ``Date`` to search for price lists of medical items with a creation date which matches completely, the typed date.

Region
  Select the ``Region`` from the list of regions by clicking on the arrow on the right of the selector to select price lists of medical items from a specific region. The option **National** means that the price list is common for all regions. *Note: The list will only be filled with the regions assigned to the current logged in user and with the option National. All nationwide pricelists and all regional pricelists relating to the selected region will be found. If no district is selected the also all district pricelists for districts belonging to the selected region will be found.*

District
  Select the ``District``;from the list of districts by clicking on the arrow on the right of the selector to select price lists medical items from a specific district. *Note: The list will be only filled with the districts belonging to the selected region and assigned to the currently logged in user. All nationwide pricelists, all regional pricelists relating to the selected region and all district pricelists for the selected district will be found.*

Show Historical Values
  Click on ``Show Historical Values`` to see historical records matching the selected criteria. Historical records are displayed in the result in grey to clearly define them from current records (:numref:`historical_values`).

  .. _historical_values:
  .. figure:: /img/user_manual/image42.png
    :align: center

    `Historical records - Result Panel`

Search button
  Once the criteria have been entered, use the search button to filter the records, the results will appear in the result panel.

Result Panel
""""""""""""

The Result Panel displays a list of all price lists of medical items found, matching the selected criteria in the search panel. Hovering over records changes the highlight to grey (:numref:`image48`). The leftmost record contains a hyperlink which if clicked, redirects the user to the actual record for detailed viewing if it is a historical record or editing if it is the current record.

.. _image48:
.. figure:: /img/user_manual/image43.png
  :align: center

  `Selected record (blue), hovered records (yellow) - Result Panel`

Information Panel
""""""""""""""""""

The Information Panel is used to display messages back to the user. Messages will occur once a price list medical item has been added, updated or deleted or if there was an error at any time during the process of these actions.

Price List Medical Item Page
============================

Data Entry
-----------

.. figure:: /img/user_manual/image44.png
  :align: center

  `Price List Medical Item Page`

Name
  Enter the name for the price list of medical items. Mandatory, 100 characters maximum.

Date
  Enter the creation date for the price list of medical items. *Note: You can also use the button next to the date field to select a date to be entered.*

Region
  Select the ``Region`` from the list of regions by clicking on the arrow on the right of the selector to enter the region in which the price list of medical items is to be used. The district **National** means that the price list is common for all regions. *Note: The list will only be filled with the regions assigned to the current logged in user and with the option National.* Mandatory.

District
  Select the ``District`` from the list of districts by clicking on the arrow on the right of the selector to enter the district in which the price list of medical items is to be used. *Note: The list will be only filled with the districts belonging to the selected region and currently logged in user.* It is not mandatory to enter a district, not selecting a district will mean the price list of medical items is used in all districts of the region or nationwide if the region National is selected .

Medical Items
  Select from the list of available medical items the medical items which the price list of medical items should contain by clicking on the ``check box`` to the left of a medical item. The list shows the medical items displaying the code, name, type and price for reference. There is also an extra column, Overrule, which can be used to overrule the pre-set price. By clicking once on the row desired item in the overrule column, a new price can be entered for the individual item. This can occur when price agreed between a health facility or group of health facilities and the health insurance administration differs from the common price in the register of medical items.

Saving
------

Once all mandatory data is entered, clicking on the ``Save`` button will save the record. The user will be re-directed back to the `Price list Medical Items Control Page <#medical-items-control-page>`__, with the newly saved record displayed and selected in the result panel. A message confirming that the price list of medical items has been saved will appear on the Information Panel.

**Mandatory data**

If mandatory data is not entered at the time the user clicks the ``Save button``, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right of the corresponding data field).

**Cancel**

By clicking on the ``Cancel`` button, the user will be re-directed to the `Price List Medical Items Control Page <#medical-items-control-page>`__.\

Adding a Price List of Medical Items
=====================================

Click on the Add button to re-direct to the `Price List Medical Item Page <#price-list-medical-item-page>`__.\

When the page opens all entry fields are empty. See the `Price List Medical Item Page <#price-list-medical-item-page>`__ for information on the data entry and mandatory fields.\

Editing a Price List of Medical Items
======================================

Click on the Edit button to re-direct to the `Price List Medical Item Page <#price-list-medical-item-page>`__\.

The page will open with the current information loaded into the data entry fields. See the `Price List Medical Item Page <#price-list-medical-item-page>`__ for information on the data entry and mandatory fields.

Duplicating a Price List of Medical Items
=========================================

Click on the Duplicate button to re-direct to the `Price List Medical Item Page <#price-list-medical-item-page>`__\.

The page will open with all the current information for the selected price list, (except for the price list name which should be unique), loaded into the data entry fields. See the `Price List Medical Item Page <#price-list-medical-item-page>`__ for information on the data entry and mandatory fields. To save the record, enter a unique code before clicking on ``Save``.

Deleting a Price List of Medical Items
=======================================

Click on the ``Delete`` button to delete the currently selected record\; the user is re-directed to the `Price List Medical Items Control Page <#medical-items-control-page>`__\.

Before deleting a confirmation popup (:numref:`pricelists_delete`) is displayed, which requires the user to confirm if the action should really be carried out?

.. _pricelists_delete:
.. figure:: /img/user_manual/pricelists_delete.png
  :align: center

  `Delete Confirmation - Button Panel`

When a price list of medical items is deleted, all records retaining to the deleted price list of medical items will still be available by selecting historical records.
