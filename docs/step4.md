> \<a href=\"<https://atmo.cyverse.org>\"
> target=\"blank\"\>Atmosphere\</a\>

> \<a
> href=\"<https://wiki.cyverse.org/wiki/display/atmman/Atmosphere+Manual+Table+of+Contents>\"
> target=\"blank\"\>Atmosphere Manual\</a\>

> \<a
> href=\"<https://learning.cyverse.org/projects/atmosphere-guide/en/latest/>\"
> target=\"blank\"\>Atmosphere Guide\</a\>

> \<a href=\"<https://bisque.cyverse.org/client_service/>\"
> target=\"blank\"\>BisQue\</a\>

> \<a href=\"<https://wiki.cyverse.org/wiki/display/BIS>\"
> target=\"blank\"\>BisQue Manual\</a\>

> \<a href=\"<https://user.cyverse.org/>\" target=\"\_blank\"\>CyVerse
> User Portal\</a\>

> \<a href=\"<http://learning.cyverse.org>\" target=\"blank\"\>CyVerse
> Learning Center\</a\>

> \<a href=\"<https://wiki.cyverse.org>\" target=\"blank\"\>CyVerse
> Wiki\</a\>

> \<a href=\"<http://www.cyverse.org/data-store>\"
> target=\"\_blank\"\>Data Store\</a\>

> \<a
> href=\"<https://wiki.cyverse.org/wiki/display/DS/Data+Store+Table+of+Contents>\"
> target=\"blank\"\>Data Store Manual\</a\>

> \<a
> href=\"<https://learning.cyverse.org/projects/data_store_guide/en/latest/>\"
> target=\"blank\"\>Data Store Guide\</a\>

> \<a href=\"<https://de.cyverse.org/de/>\" target=\"blank\"\>Discovery
> Environment\</a\>

> \<a
> href=\"<https://wiki.cyverse.org/wiki/display/DEmanual/Table+of+Contents>\"
> target=\"blank\"\>DE Manual\</a\>

> \<a
> href=\"<http://learning.cyverse.org/projects/cyverse-discovery-environment-guide/>\"
> target=\"blank\"\>Discovery Environment Guide\</a\>

> \<a href=\"<https://dnasubway.cyverse.org/>\" target=\"blank\"\>DNA
> Subway\</a\>

> \<a
> href=\"<https://learning.cyverse.org/projects/dnasubway_guide/en/latest/>\"
> target=\"blank\"\>DNA Subway Manual\</a\>

> \<a
> href=\"<https://learning.cyverse.org/projects/dnasubway_guide/en/latest/>\"
> target=\"blank\"\>DNA Subway Guide\</a\>

> \<a href=\"<https://www.sciapps.org/>\"
> target=\"blank\"\>SciApps\</a\>

> \<a
> href=\"<https://learning.cyverse.org/projects/sciapps_guide/en/latest/>\"
> target=\"blank\"\>SciApps Manual\</a\>

> \<a
> href=\"<https://learning.cyverse.org/projects/sciapps_guide/en/latest/>\"
> target=\"blank\"\>SciApps Guide\</a\>

> \<a href=\"<https://cyverse-de.github.io/api/>\"
> target=\"blank\"\>Terrain DE API Docs\</a\>

> \<a
> href=\"<https://tacc-cloud.readthedocs.io/projects/agave/en/latest/>\"
> target=\"blank\"\>Tapis TACC API Docs\</a\>

> \<a href=\"<http://ask.iplantcollaborative.org/questions>\"
> target=\"blank\"\>Ask CyVerse\</a\>

> \<a href=\"<http://learning.cyverse.org/en/latest/>\"
> target=\"blank\"\>Agave Guide\</a\>

> \<a href=\"<http://developer.agaveapi.co/#introduction>\"
> target=\"blank\"\>Agave API\</a\>

> \<a href=\"<https://agaveapi.co>\" target=\"blank\"\>Agave Live
> Docs\</a\>

> \<a href=\"<http://learning.cyverse.org/en/latest/>\"
> target=\"blank\"\>BisQue Guide\</a\>

\_

![Home_Icon](./img/homeicon.png){width="25px" height="25px"}\_ [Learning
Center Home](http://learning.cyverse.org/)

**Transferring Data to and from an Instance**
\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--

An Atmosphere instance only contains data that were included in the
original image that was used to make that instance. You can transfer
data to/from the CyVerse Data Store, an Atmosphere Volume, a sever, or
your local machine. In this guide, we will only cover data transfer
using iCommands. iCommands is installed on every Atmosphere instance.

**Related Links**

-   **iCommands Guide:**
    [link](https://cyverse-data-store-guide.readthedocs-hosted.com/en/latest/step2.html)
-   **iCommands Download:**
    [link](https://wiki.cyverse.org/wiki/display/DS/Setting+Up+iCommands)

------------------------------------------------------------------------

# *Transferring Data to/from an Instance using iCommands*

You can execute to the instance\'s icommand if you are connected via
SSH/PuTTY or if you are connected to the desktop via VNC, open the
instance\'s terminal application.

> 1.  At the instance\'s terminal, start the iCommands configuration
>     using the \'iinit\' command and enter configure.
>
>     > ::: important
>     > ::: title
>     > Important
>     > :::
>     >
>     > This configuration is a one-time step on your first use with
>     > this instance.
>     >
>     > ``` bash
>     > $ iinit
>     >
>     > # As prompted, enter the following values:
>     > # Host: data.cyverse.org
>     > # Port: 1247
>     > # User: your_cyverse_username
>     > # Zone: iplant
>     > # Password: your_cyverse_password
>     > ```
>     >
>     > If you make a mistake in your configuration you can edit
>     > [\~/.irods/irods_environment.json]{.title-ref} on your instance.
>     > :::
>
> 2.  Test your configuration by listing your Data Store contents with
>     the \"ils\" command.
>
>     > ``` bash
>     > $ ils
>     > ```
>     >
>     > ::: tip
>     > ::: title
>     > Tip
>     > :::
>     >
>     > If you made a mistake during the configuration, you can edit
>     > your icommands configuration file.
>     > :::
>
> 3.  To download a file from the Data Store to your instance, use
>     \"iget\"
>
>     > ``` bash
>     > $iget data_store_file
>     > ```
>
> 4.  To upload file from your instance to the Data Store use \"iput\"
>
>     > ``` bash
>     > $iget file_on_instance location_on_data_store
>     > ```

::: tip
::: title
Tip
:::

iCommands has a variety of options, to see progress of transfers,
operate recursively, and more. See additional [iCommands
documentation](https://wiki.cyverse.org/wiki/display/DS/Using+iCommands)
on the CyVerse wiki.
:::

------------------------------------------------------------------------

**Fix or improve this documentation**

-   Search for an answer:
-   Ask us for help: click on the lower right-hand side of the page
-   Report an issue or submit a change:
-   Send feedback: [Tutorials@CyVerse.org](Tutorials@CyVerse.org)

------------------------------------------------------------------------

> ![Home_Icon](./img/homeicon.png){width="25px" height="25px"}\_
> [Learning Center Home](http://learning.cyverse.org/)
