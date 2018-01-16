# Plugin [Interface] - Combo Box Control

## Syntax

```pebakery
<Name>=<Value>,<Visibility>,4,<PosX>,<PosY>,<Width>,<Height>,<Option1>,<Option2>,<OptionN>[,<SectionToRun>,<ShowProgress>][,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Value | The value currently selected by the combo box. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| Option | Options to display in the combo box. Multiple values are separated by commas. |
| SectionToRun | **(Optional)** Defines the [Section] that will be processed when the button is pressed or the value of the control is changed. The section name must be enclosed in underscore `_` characters. |
| ShowProgress | **(Optional)** True/False - Show the Build progress screen. This argument must always follow the `SectionToRun` argument. |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. |