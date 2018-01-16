# Plugin [Interface] - Number Box Control

## Syntax

```pebakery
<Name>=<Name>,<Visibility>,2,<PosX>,<PosY>,<Width>,<Height>,<Value>,<Min>,<Max>,<Increment>[,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| Min | The minimum value the number box will allow. |
| Max | The maximum value the number box will allow. |
| Increment | Clicking the up/down arrows on the number box will increase the value by a factor of X. |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. |

## Remarks

## Related

## Examples