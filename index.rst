|CyVerse logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

Atmosphere
==========

Goal
----

`Atmosphere <http://www.cyverse.org/atmosphere>`_ is one of the most versatile
components of the CyVerse CI. Anything that you would normally be able to do
with your local laptop/desktop, you can do on a virtual machine in the
Atmosphere cloud. This guide will cover the basics you need to get started
using Atmosphere. For the full documentation, see the `Atmosphere Manual <https://wiki.cyverse.org/wiki/display/atmman/Atmosphere+Manual+Table+of+Contents>`_
on the CyVerse wiki.

----

.. toctree::
	:maxdepth: 2

	Tutorial home <index.rst>
	Logging in to Atmosphere <step1.rst>
	Creating a Project and Launching an Instance <step2.rst>
	Connecting to an Instance <step3.rst>
	Transfering Data to/from an Instance <step4.rst>
	Terminating an Instance <step5.rst>

..
	#### Comment:This tutorial can have multiple pages. The table of contents assumes
	you have an additional page called 'First Step' with content located in 'step1.rst'.
	Copy step1.rst. step2.rst has sligtly different formatting to end the document.
	Edit these titles and filenames as needed ####


Prerequisites
-------------


Downloads, access, and services
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*In order to complete this tutorial you will need access to the following services/software*

..
	#### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Preparation/Notes
      - Link/Download
    * - CyVerse account
      - You will need a CyVerse account to complete this exercise
      - `Register <https://user.cyverse.org/>`_
		* - Atmosphere Access
			- Atmosphere access is by request only
			- Check or request access: `CyVerse User Portal <https://user.cyverse.org/services/mine>`_
		* - iCommands (Optional)
			- While you don't have to have iCommands installed, the transfering data
				section of this guide assumes familiarity with iCommands. You may wish
				to complete the iCommands tutorial, and you may wish to install iCommands
				on a local machine if you want to transfer data from that machine to an
				Atmosphere instance
			- - `iCommands Quick Start <>`_
				- `iCommands Download links <>`_
		* - Terminal or SSH client (Optional)
			-	You can connect via Webshell to an Atmosphere instance from a web
				browser. Alternatively, you can connect via SSH from a Mac or Linux
				computer. If you are using Windows, we suggest a SSH client.
			-  Windows compatible SSH client (Optional) `PuTTY <https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html>`_
		* - VNC Viewing Client (Optional)
			- You can connect to a desktop-enabled Atosphere instance from a web
				browser. Alternatively you can connect via a VNC viewing client such as
				Real VNC viewer.
			- Download `Real VNC Viewer for your OS <https://www.realvnc.com/download/viewer/>`_

.. Tip::
		To request access to Atmosphere, login to the `CyVerse User Portal`_.
		In the `Services Menu <https://user.cyverse.org/services/mine>`_ under 'MY
		SERVICES' you should see Atmosphere listed as an option you can launch. If
		not, Look uner the `Available <https://user.cyverse.org/services/available>`_
		menu, and click the 'REQUEST ACCESS' link. You will recive an email
		requesting additional information. To qualify for an Atmosphere account,
		your CyVerse account must be associated with an institutional email address
		(e.g. .edu/.org/.gov).

----

**Fix or improve this documentation**

- On Github: `Repo link <https://github.com/CyVerse-learning-materials/atmosphere_guide>`_
- Send feedback: `Tutorials@CyVerse.org <Tutorials@CyVerse.org>`_

----

|Home_Icon|_
`Learning Center Home`_

.. |CyVerse logo| image:: ./img/cyverse_rgb.png
    :width: 500
    :height: 100
.. _CyVerse logo: http://learning.cyverse.org/
.. |Home_Icon| image:: ./img/homeicon.png
    :width: 25
    :height: 25
.. _Home_Icon: http://learning.cyverse.org/
