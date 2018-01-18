# Image Control

## Syntax

```pebakery
<Name>=<Image>,<Visibility>,5,<PosX>,<PosY>,<Width>,<Height>[,<ToolTip>]
```

### Arguments

| Argument | Description |
| --- | --- |
| Name | Unique name used to reference this control. |
| Image | The name of the encoded image to display on the control. (*.png; *.jpg; *.gif; *.bmp; *.ico) are supported. |
| Visibility | True/False - Show or Hide the control. |
| ControlID | The control ID specifying the type of the control. |
| PosX | Horizontal Position measured from the control's top left corner. |
| PosY | Vertical Position measured from the control's top left corner. |
| Width | Width of the control. |
| Height | Height of the control. |
| URL | The website to launch if the image is clicked. |
| ToolTip | **(Optional)** Help Text that will be shown when the user hovers over the control. This argument must always begin with a double underscore `__`. *Example:* `"__Some useful info"` |

## Remarks

If a `URL` is not defined clicking on the image will open it in the operating systems default image viewer.