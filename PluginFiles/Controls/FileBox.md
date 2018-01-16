# Plugin [Interface] - File Box Control

## Syntax

```pebakery
<Name>=<Value>,<Visibility>,13,<PosX>,<PosY>,<Width>,<Height>[,FILE][,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Value | The path currently entered in the File Box. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| FILE | **(Optional)** If specified the browse button will display a directory selection dialog instead of a file selection dialog. |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. |