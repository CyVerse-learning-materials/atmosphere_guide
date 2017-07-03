|CyVerse logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


**Transferring Data to and from an Instance**
--------------------------------------------

An Atmosphere instance only contains data that were included in the original
image that was used to make that instance. You can transfer data to/from
the CyVerse Data Store, an Atmosphere Volume, a sever, or your local machine.
In this guide, we will only cover data transfer using iCommands. iCommands is
installed on every Atmosphere instance.


**Related Links**

.. #### Comment: Optional - Insert platform logo

- **iCommands Guide:** `link <https://cyverse-data-store-guide.readthedocs-hosted.com/en/latest/step2.html>`_
- **iCommands Download:** `link <https://wiki.cyverse.org/wiki/display/DS/Setting+Up+iCommands>`_


----

*Transferring Data to/from an Instance using iCommands*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can execute to the instance's icommand if you are connected via SSH/PuTTY or
if you are connected to the desktop via VNC, open the instance's terminal
application.


  1. At the instance's terminal, start the iCommands configuration using the
     'iinit' command and enter configure.

      .. important::
          This configuration is a one-time step on your first use with this
          instance.

        .. code:: bash

          $ iinit

          # As prompted, enter the following values:
          # Host: data.cyverse.org
          # Port: 1247
          # User: your_cyverse_username
          # Zone: iplant
          # Password: your_cyverse_password

        If you make a mistake in your configuration you can edit `~/.irods/irods_environment.json`
        on your instance.

  2. Test your configuration by listing your Data Store contents with the "ils"
     command.

      .. code:: bash

        $ ils

      .. Tip::
          If you made a mistake during the configuration, you can edit your
          icommands configuration file.

  3. To download a file from the Data Store to your instance, use "iget"

      .. code:: bash

        $iget data_store_file

  4. To upload file from your instance to the Data Store use "iput"

      .. code:: bash

        $iget file_on_instance location_on_data_store


.. tip::
    iCommands has a variety of options, to see progress of transfers, operate
    recursively, and more. See additional `iCommands documentation <https://wiki.cyverse.org/wiki/display/DS/Using+iCommands>`_ on the
    CyVerse wiki.


..
	#### Comment: Suggested style guide:
	1. Steps begin with a verb or preposition: Click on... OR Under the "Results Menu"
	2. Locations of files listed parenthetically, separated by carets, ultimate object in bold
	(Username > analyses > *output*)
	3. Buttons and/or keywords in bold: Click on **Apps** OR select **Arabidopsis**
	4. Primary menu titles in double quotes: Under "Input" choose...
	5. Secondary menu titles or headers in single quotes: For the 'Select Input' option choose...
	####


----

**Fix or improve this documentation:**

- On Github: `Repo link <https://github.com/CyVerse-learning-materials/atmosphere_guide>`_
- Send feedback: `Tutorials@CyVerse.org <Tutorials@CyVerse.org>`_

----

  |Home_Icon|_
  `Learning Center Home <http://learning.cyverse.org/>`_

.. |CyVerse logo| image:: ./img/cyverse_rgb.png
    :width: 500
    :height: 100
.. _CyVerse logo: http://learning.cyverse.org/
.. |Home_Icon| image:: ./img/homeicon.png
    :width: 25
    :height: 25
.. _Home_Icon: http://learning.cyverse.org/
