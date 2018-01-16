# Radio Group Control

## Syntax

```pebakery
<Name>=<Caption>,<Visibility>,14,<PosX>,<PosY>,<Width>,<Height>,<Item1>,<Item2>,<ItemN>,<SelectedIndex>[,<SectionToRun>,<ShowProgress>][,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Caption | Label displayed on the top of the radio group. Use `""` for none. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| Option | Options to display in radio group. Multiple values are separated by commas. |
| SelectedIndex | Zero-based index of the selected `Option`. |
| SectionToRun | **(Optional)** Defines the [Section] that will be processed when the button is pressed or the value of the control is changed. The section name must be enclosed in underscore `_` characters. |
| ShowProgress | **(Optional)** True/False - Show the Build progress screen. This argument must always follow the `SectionToRun` argument. |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. |

## Remarks

## Related

## Examples