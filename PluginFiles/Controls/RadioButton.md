# Radio Button Control

## Syntax

```pebakery
<Name>=<Caption>,<Visibility>,11,<PosX>,<PosY>,<Width>,<Height>,<Value>[,<SectionToRun>,<ShowProgress>][,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Caption | Label displayed next to the radio button. Use `""` for none. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| Value | True/False - Selected `True` Deselected `False` |
| SectionToRun | **(Optional)** Defines the [Section] that will be processed when the button is pressed or the value of the control is changed. The section name must be enclosed in underscore `_` characters. |
| ShowProgress | **(Optional)** True/False - Show the Build progress screen. This argument must always follow the `SectionToRun` argument. |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. |

## Remarks

## Related

## Examples