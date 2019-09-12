.. include:: /_sidebar.rst.inc

Funding
^^^^^^^

  Access to the ``Funding`` is restricted to the users with the system role of Accountant or with a role including an access to Tools/Funding.

  The ``Funding`` is the place where funding from external authorities (payers) can be for entered. openIMIS creates internally one fictive family/group (the insurance number of the head of the fictive family/group is 999999999, the name is *Funding* and the other name is *Funding* as well) for the district for which a funding is done. Each entering of a fund results in creation of a fictive policy for the corresponding fictive family/group with paid contribution in the amount of the funding. The fictive policy is active since the date of payment of the corresponding fund. These fictive policies are overpaid as these funds are usually much higher than the contribution rate for a single family/member of the group but it doesn’t matter. External funding corresponds to payment of contributions for many families/members of the group in some period. openIMIS can regard funds as standard contributions and its standard functionality can be used for handling of funds. One distinctive feature of payment of funds by means of the fictive policies is that the payments of funds don’t appear in the reports on matching funds generated for funding authorities. So, there is no danger that offices of the scheme administration would acquire new funds based on funding already acquired.

Navigation
""""""""""

  The functionality for entering of funds can be found under the main menu ``Tools``, sub menu ``Funding``

  .. _image247:
  .. figure:: /img/user_manual/image214.png
    :align: center

    `Image 247 - Navigation Funding`

  Clicking on the sub menu ``Funding`` re-directs the current user to the `Funding Page. <#image-6.79-funding-page>`__

Funding Page
""""""""""""

 #. **Data Entry**

    .. _image248:
    .. figure:: /img/user_manual/image215.png
      :align: center

      `Image 248 - Funding Page`

    * ``Region``

      Select the region from the list of regions for which the funding is designated by clicking on the arrow on the right of the selector. *Note: The list will only be filled with the regions assigned to the current logged in user.*

    * ``District``

      Select the district from the list of districts for which the funding is designated. by clicking on the arrow on the right of the selector. *Note: The list will only be filled with the districts belonging to the selected region and assigned to the current logged in user.*

    * ``Product``

      Select an insurance product from the list of insurance products purchased in the selected district (including national insurance products) for which the funding is designated.

    * ``Payer``

      Select from the list of institutional payers the funding authority/agency.

    * ``Payment Date``

      Enter the date of receiving of the funding.

    * ``Contribution Paid``

      Enter the amount of the funding.

    * ``Receipt Number``

        Enter an identification of the document accompanying the funding.

 #. **Saving**

    Once all mandatory data is entered, clicking on the ``Save`` button will save the record. A message confirming that the new password has been saved will appear. The user will be re-directed back to the `Home Page <#image-2.2-home-page>`__.

 #. **Mandatory data**

    If mandatory data is not entered at the time the user clicks the ``Save`` button, a message will appear in the Information Panel, and the data field will take the focus (by an asterisk on the right side of the corresponding field). The user will be re-directed to the `Home Page <#image-2.2-home-page>`__.

 #. **Cancel**

    By clicking on the Cancel button, the user will be re-directed to the `Home Page <#image-2.2-home-page>`__.
