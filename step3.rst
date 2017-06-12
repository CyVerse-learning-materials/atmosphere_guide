|CyVerse logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


Connecting to an Instance
-------------------------

Once your instance is in the 'Active' state, you can connect to the instance.
All instances support connection at the command line via SSH. Many (but not all)
instances may also have a graphical desktop. You can connect to these desktops
via a VNC viewing client. We will cover both methods in this guide.

----

**Connect to Atmosphere Instance using SSH**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Connecting using Mac or Linux Terminal**
``````````````````````````````````````````

1. If necessary, login to `Atmosphere <https://atmo.cyverse.org/>`_. and locate
   the instance you are connecting to in a given project.

2. Locate the IP address and copy this to your clipboard.

3. Open your computer's terminal application.

4. Connect via SSH:

    .. code:: bash

      $ ssh your_cyverse_username@your.atmosphere.ip.address

      # If connecting for the first time, you may be get a security prompt

      The authenticity of host '128.196.64.200 (128.196.64.200)' can\'t be established.
      ECDSA key fingerprint is SHA256:fzEJLqeljHgIwcGY0gUap2sRWLlGPQwUVimhEgkJYBs.
      Are you sure you want to continue connecting (yes/no)?

      # you may accept this prompt by typing yes

5. You will be prompted to enter your CyVerse password

    .. Tip::
       Your cursor will not move or indicate you are typing as you enter your
       password. If you make a mistake, hit enter and you will be prompted again.

You should now be connected to your Atmosphere instance.


**Connecting using Windows and PuTTY**
``````````````````````````````````````

1. If necessary, login to `Atmosphere <https://atmo.cyverse.org/>`_. and locate
   the instance you are connecting to in a given project.

2. Locate the IP address and copy this to your clipboard.

3. Open 'PuTTY.exe' and paste the IP address into the 'Host Name (or IP addres
   s)' field; click 'Open'

    .. note::
      If this is your first time connecting, you may get a security prompt that
      the server's host key is not chached in the registry. You may click 'Yes'
      to continue connecting.

4. When prompted, enter your CyVerse username for the request to 'login as:'
   and enter your CyVerse password to connect.

   .. Tip::
      Your cursor will not move or indicate you are typing as you enter your
      password. If you make a mistake, hit enter and you will be prompted again.



**Connect to Atmosphere Instance using VNC viewer**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. note::

   You can only connect to an Atmosphere instance that has a desktop installed
   and has a running VNC server. Usually this information is in the image
   description. If you are unsure, or having difficulty in connecting to and
   instance you belive should have a desktop, contact Atmosphere support.

   If you have not already done so, download `Real VNC Viewer <https://www.realvnc.com/download/viewer/>`_

1. If necessary, login to `Atmosphere`_. and locate the instance you are
   connecting to in a given project.

2. Locate the IP address and copy this to your clipboard.

3. Open VNC Viewer. Paste your **IP address + “:1”** in the ‘VNC Server’ field
   (e.g. 161.803.39.887:1) and click connect.

   .. note:: When connecting for the first time to an instance, you will be
      prompted to save a signature

4. When prompted, ensure your username entered is your CyVerse username. Enter
   your CyVerse password and click Ok.

You should now be connected to your instance desktop.

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
