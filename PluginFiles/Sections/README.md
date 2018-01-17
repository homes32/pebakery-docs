# Plugin File Sections

The structure of a .script file consists of 4 major sections. Additional sections may be defined by the plugin author to included additional commands, interfaces, or embedded files.

## Sections

### Main Sections

The following sections define the behavior and actions of the plugin. Click on a `Section` name for more details.

| Section | Description |
| --- | --- |
| [Main](./Main.md) | The main section that defines your plugin. |
| [Interface](./Interface.md) | **(Optional)** The Interface section contains one ore more lines that define the controls of a Plugin's Graphical User Interface.  |
| [Process](./Process.md) | **(Optional)** This sections contains the main logic of the plugin and is processed when you press the `Build` button. |
| [Variables](./Variables.md) | **(Optional)** This section is used to predefine variables and macros used by the plugin at runtime. |

### Internal Sections

The following sections are used internally by PEBakery and should not be modified.

| Section | Description |
| --- | --- |
| InterfaceEncoded | Contains a list of encoded files used by the Plugin's Graphical User Interface |
| `EncodedFile-InterfaceEncoded-<FileName>` | Contains the encoded file referenced by `FileName` from the `InterfaceEncoded` section. |
| AuthorEncoded | Defines the plugin's logo image. |
| `EncodedFile-AuthorEncoded-<FileName>` | Contains the encoded file for the plugin's logo image. |
