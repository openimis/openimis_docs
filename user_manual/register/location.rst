Locations
^^^^^^^^^

  Administration of locations is restricted to users with the the system role of IMIS Administrator or with a role including an access to Administration/Locations. The user can see only locations he/she has access to.

Pre-conditions
""""""""""""""

  A region, district, municipality or village may only be added or thereafter edited, after the approval of the management of the scheme administration.

Navigation
""""""""""

  All functionality for use with the administration of locations can be found under the main menu ``Administration``, sub menu ``Locations.``

  .. _location_menu:
  .. figure:: /img/user_manual/location.menu.png
    :align: center

    `Navigation Locations`

  Clicking on the sub menu ``Locations`` redirects the current user to the `Locations Page. <#locations-page>`__

  .. _location_search:
  .. figure:: /img/user_manual/location.search.png
    :align: center

    `Locations Page`

Locations Page
""""""""""""""

  The Locations page is the central point for all locations administration. By having access to this page, it is possible to add, edit, delete and move regions, districts, municipalities and villages. The page is divided into three panels (:numref:`location_search`). *Note. Only regions and districts with associated municipalities and villages, belonging to the logged in user will be available to edit or delete. On adding a new region or district, the user will automatically become associated with this region or district*.


 #. **Locations Panel**

    This is the working panel and is divided into four vertical panels of ``Regions``, ``Districts``, ``Municipalities`` and ``Villages.``

 #. **Button Panel**

    It has three buttons, ``Add`` (:numref:`mat_add`), ``Delete`` (:numref:`mat_delete`) and ``Move`` (:numref:`mat_move`) for actions on the locations, double click on a location will open the edit modal box.

      .. _mat_buttons_loc:
      .. list-table:: Material design button
        :widths: 1 1 1

        * - .. _mat_move:
            .. figure:: /img/user_manual/mat.move.png
              :align: center

              'Move'
          - .. _mat_refresh:
            .. figure:: /img/user_manual/mat.refresh.png
              :align: center

              `Refresh`
          - .. _mat_delete:
            .. figure:: /img/user_manual/mat.delete.png
              :align: center

              `Delete`

 #. **Information Panel**

    The Information Panel is used to display messages back to the user. Messages will occur once a region, district or municipality or village has been added, updated, moved or deleted or if there was an error at any time during the process of these actions.


Adding a Region, District, Municipality, Village
""""""""""""""""""""""""""""""""""""""""""""""""

  Focusing on the appropriate level of locations by clicking on the ``Add`` button will open up a modal entry box. Here one could enter the new code (**Code**) and name (**Name**) of a region, district, municipality or village. For villages, the number of male inhabitants (**M**), female inhabitants (**F**), inhabitants with the unspecified gender (**O**) and the number of families (**Fam.**) can be specified. On clicking the ``Save`` button the new record will be saved.

Editing a Region, District, Municipality, Village
"""""""""""""""""""""""""""""""""""""""""""""""""

  Selecting the location to edit and clicking on the ``Edit`` button will open up in the top of the screen an entry box with the name of the location. Here one could change the name. On clicking the ``Save`` button, the record will be saved.

Deleting a Region, District, Municipality, Village
""""""""""""""""""""""""""""""""""""""""""""""""""

  Select first the location to delete and click the ``Delete`` button. *Note. It is not possible to delete a region, district or municipality with associated districts, municipalities or villages respectively.*

  Before deleting a confirmation popup (:numref:`location.delete_conf`) is displayed, which requires the user to confirm if the action should really be carried out?

  .. _location.delete_conf:
  .. figure:: /img/user_manual/location.delete_conf.png
    :align: center

    `Delete confirmation – Location Page`

  When a region, district, municipality or village is deleted, all records retaining to the deleted region, district, municipality or village will still be available by selecting historical records.

Moving a District, Municipality, Village
""""""""""""""""""""""""""""""""""""""""

  Moving of a location is needed when the administrative division of the territory, on which a health insurance scheme is active, changes. Clicking on the ``Move`` button will open the move location box (:numref:`location_move`).

  .. _location_move:
  .. figure:: /img/user_manual/location.move.png
    :align: center

    `Move Location Page`


 #. **Move Location box**

    The move location box is composed of three sections, the first display the name of the location to be moved. The second display the name of the current parent when the third enable the selection of the future parents.

    For moving a location, select the new parents (village, municipality, district), the fields will appear when needed, for example the municipality drop-down list will be displayed only if the district is selected. The level of the location can be changed by choosing the lower (resp. higher) parent having a different level from the current parent; be aware that the lowest location is the village, therefore if a municipality is moved to village level then the villages under the moved municipality will remain villages but will be moved under the municipality chosen the new parent of the to-be moved municipality.

    The Move will be effective once the ``Move`` button is clicked.




