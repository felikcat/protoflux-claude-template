# Component:Slider`1

> Source: https://wiki.resonite.com/Component:Slider`1

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Slider%601&diff=88792) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8c/Slider%601Component.png/510px-Slider%601Component.png)](https://wiki.resonite.com/File:Slider%601Component.png) **Slider\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Slider** component is a [UIX](https://wiki.resonite.com/UIX "UIX") element that a [user](https://wiki.resonite.com/User "User") can use to grab and move along a line, returning a value of that slider's position.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want a 3D slider, use the [Slider](https://wiki.resonite.com/Component:Slider "Component:Slider") component instead.


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color for this slider. |
| `ColorDrivers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ColorDriver](https://wiki.resonite.com/index.php?title=Type:ColorDriver&action=edit&redlink=1 "Type:ColorDriver (page does not exist)")** | Gives extra color control for different color drive targets. |
| `__legacy_NormalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Internal - Legacy normal color. |
| `__legacy_HighlightColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Internal - Legacy highlight color. |
| `__legacy_PressColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Internal - Legacy press color. |
| `__legacy_DisabledColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Internal - Legacy disabled color. |
| `__legacy_TintColorMode` | **[ColorMode](https://wiki.resonite.com/index.php?title=Type:ColorMode&action=edit&redlink=1 "Type:ColorMode (page does not exist)")** | Internal - Legacy tint color mode. |
| `__legacy_ColorDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Internal - Legacy color drive. |
| `IsPressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Check if the user is pressing on the slider handle. |
| `IsHovering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Check if the user is hovering on the slider handle. |
| `Value` | **T** | The position this slider is at (normalized between `0` and `1`) |
| `Min` | **T** | The minimum value of this slider. |
| `Max` | **T** | The maximum value of this slider. |
| `Integers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Changes the way this slider counts along the slider line. Setting to integers makes it step along whole numbers. |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Changes the way this slider determines its position. Power represents a shifted curve of values that is heavier at the ends of the slider. |
| `Clamp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enforces the min and max values of this slider. |
| `VibrationThreshold` | **T** | Haptic feedback for this slider. |
| `SlideDirection` | **[Direction](https://wiki.resonite.com/Component:Slider%601#Direction) <T>** | The orientation of this slider's direction. |
| `AnchorOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset for the handle of this slider. |
| `HandleAnchorMinDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The min offset for the handle drive. |
| `HandleAnchorMaxDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The man offset for the handle drive. |
| `FillLineDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | Fill line for this slider, fills in one side of it. |
| `RequireLockInToInteract` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Checks to see if a user has locked in a press on this slider. |
| `RequireInitialPress` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Check for a initial press from a user. |

Fields
Collapse

## Usage

Sliders are very useful for making menus that do not need to be precise on [UIX](https://wiki.resonite.com/UIX "UIX") elements (unless using steps to lock into a value).

## Examples

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime") has made a tutorial on sliders for [UIX](https://wiki.resonite.com/UIX "UIX"):

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Slider%601&oldid=88792](https://wiki.resonite.com/index.php?title=Component:Slider%601&oldid=88792)"

Contents