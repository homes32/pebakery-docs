# Text Label Control

## Syntax

```pebakery
<Name>=<Caption>,<Visibility>,1,<PosX>,<PosY>,<Width>,<Height>,<FontSize>,<FontWeight>[,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Caption | Text displayed on the control. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| Font Size | Font Size in points. (ex. 12) |
| Font Weight | Can be `Normal` or `Bold` |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. *Example:* `"__Some useful info"` |

## Remarks
