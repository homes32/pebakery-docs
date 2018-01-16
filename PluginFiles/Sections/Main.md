# Plugin [Main] Section

The main section that defines all the details of your plugin. This data affects how your plugin is displayed in PEBakerys user interface as well as how it is processed during a build.

## Syntax

Plugin data is stored in .INI style `Key=Value` format.

## Values

| Name | Description |
| --- | --- |
| Title | The title of your plugin. |
| Description | **(Optional)** A short description of the plugins intended purpose. |
| Author | **(Optional)** The author of the plugin. |
| Credits | **(Optional)** Acknowledgment of people or teams that contributed to the plugin's development. |
| Date | **(Optional)** Date the plugin was released. (Recommended format is YYYY-MM-DD.) |
| Version | **(Optional)** Version number of the plugin. |
| Level | **(Optional)** Defines the sequence in which the plugin is processed. Default is `5`.|
| Selected | **(Optional)** Defines how the plugin can be selected for processing. Default is `True`. |
|| True - The plugin is selected in the project tree and will be processed. |
|| False - The plugin is deselected in the project tree and will not be processed. |
|| None - The plugin is not allowed to be selected/deselected and will not be processd. Used primarily for configuration and utility plugins. |
| Interface | **(Optional)** Specifies the section that contains the currently displayed Graphical User Interface of the plugin. Default is `Interface`. |
| Mandatory | **(Optional)** The plugin will be processed and cannot be disabled. Default is `False`.|


