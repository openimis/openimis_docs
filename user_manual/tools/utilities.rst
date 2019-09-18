

Utilities
^^^^^^^^^

  Access to the ``Utilities`` is restricted to the users with the role of openIMIS Administrator.

  The ``Utilities`` is the place for database administration. By having access to this page, it is possible to backup and restore the openIMIS operational database and also to execute SQL Scripts (patches provided for maintenance or update of the database). At the top of the page, the current “Backend” version is displayed for reference.

Navigation
""""""""""

  All functionality for use with the administration of utilities can be found under the main menu ``Tools``, sub menu ``Utilities``

  .. _image243:
  .. figure:: /img/user_manual/image211.png
    :align: center

    `Image 243 - Navigation Utilities`

  Clicking on the sub menu ``Utilities`` re-directs the current user to the `Utilities Page. <#image-6.75-utilities-page>`__

  .. _image244:
  .. figure:: /img/user_manual/image212.png
    :align: center

    `Image 244 - Utilities Page`

Backup
""""""

  Backup utility can be found in the top panel of the `Utilities Page <#Utilities>`_. By default the path of the backup folder will be populated from the default table. User can change the path according to the requirement. Next to the textbox user can see one heck box called ``Save Path``. If user wants to update the backup folder in default table then this check box should be in checked state. Otherwise system will take the backup on the folder assigned by the user but it will not be updated in database. So next time when user comes on the `Utilities Page <#Utilities>`_, the textbox will be populated with the original path. After the path has been entered user can just click on the ``Backup button`` to start the process and a progress bar will be appeared on the screen. Users are requested to be patient while the system performs the task.

  .. _image245:
  .. figure:: /img/user_manual/image213.png
    :align: center

    `Image 245 - Backup is in progress`

Restore
"""""""

  Restore utility can be found in the second panel of the `Utilities Page <#Utilities>`_. User will have to put the path of the backup file to be restored. After the path has been entered user can just click on the ``Restore`` button to start the process and a progress bar will be appeared on the screen. Users are requested to be patient while the system performs the task.

  .. _image246:
  .. figure:: /img/user_manual/image213.png
    :align: center

    `Image 246 - Backup is in progress`

Execute script
""""""""""""""

  Execute script can be found in the third panel of the `Utilities Page <#Utilities>`_. User will have to choose the script by clicking on the browse button. User will have to select the file only with the ".isf" extension. After the file has been chosen, user can just click on the ``Execute`` button to run the script. Users are requested to be patient while the system is executing the script. After the script is executed successfully, backed version will be updated to the latest version. If user will try to run the lower or the equal version's script then system will prompt the user with the appropriate message.
