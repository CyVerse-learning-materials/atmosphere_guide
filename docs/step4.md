# Transferring Data to and from an Instance

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

## Transferring Data to/from an Instance using iCommands

You can execute to the instance's icommand if you are connected via
SSH/PuTTY or if you are connected to the desktop via VNC, open the
instance's terminal application.

> 1.  At the instance's terminal, start the iCommands configuration
>     using the 'iinit' command and enter configure.
>
>       
>     > > **Important**
>     > > 
>     > > This configuration is a one-time step on your first use with
>     > > this instance.
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
>     > [~/.irods/irods_environment.json]{.title-ref} on your instance.
>
> 2.  Test your configuration by listing your Data Store contents with
>     the "ils" command.
>
>     > ``` bash
>     > $ ils
>     > ```
>     >
>     > > **Tip**
>     >
>     > > If you made a mistake during the configuration, you can edit
>     > > your icommands configuration file.
>
> 3.  To download a file from the Data Store to your instance, use
>     "iget"
>
>     > ``` bash
>     > $ iget data_store_file
>     > ```
>
> 4.  To upload file from your instance to the Data Store use "iput"
>
>     > ``` bash
>     > $ iget file_on_instance location_on_data_store
>     > ```

> **Tip**
>
> iCommands has a variety of options, to see progress of transfers,
> operate recursively, and more. See additional [iCommands documentation](https://wiki.cyverse.org/wiki/display/DS/Using+iCommands)
> on the CyVerse wiki.


------------------------------------------------------------------------

**Fix or improve this documentation**

-   Search for an answer: [CyVerse Learning Center](https://learning.cyverse.org/en/latest/)
-   Ask us for help: click on the lower right-hand side of the page
-   Report an issue or submit a change: [GitHub Repo Link](https://github.com/CyVerse-learning-materials/atmosphere_guide/tree/mkdocs)
-   Send feedback: [learning@CyVerse.org](learning@CyVerse.org)

------------------------------------------------------------------------

[Learning Center Home](http://learning.cyverse.org/)