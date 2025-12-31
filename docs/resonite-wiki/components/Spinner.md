# Component:Spinner

> Source: https://wiki.resonite.com/Component:Spinner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Spinner&diff=113930) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b4/SpinnerComponent.png/510px-SpinnerComponent.png)](https://wiki.resonite.com/File:SpinnerComponent.png) **Spinner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Spinner** component is used to make something rotate on 1 or more axis at a constant rate.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Range` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | how much each axis can go up to from 0 before wrapping around. |
| `_target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field to spin. |
| `_offset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | the offset rotation to start at world start from. |
| `_speed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | how fast to rotate on each axis, in Degrees per Second. Negative values go in reverse. |

Fields
Collapse

## Usage

Note: While this component works very well for fixed or discrete speed steps, it might not behave as expected when the speed field is continuously changing, even a very small change can cause the component to 'jerk' on each change.

If you want to make something speed up or slow down smoothly, one option is to use rotational maths to recreate this component in flux, for example using [ProtoFlux:AxisAngle](https://wiki.resonite.com/ProtoFlux:AxisAngle "ProtoFlux:AxisAngle")

## Examples

Spinner tutorial by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime").

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Spinner&oldid=113930](https://wiki.resonite.com/index.php?title=Component:Spinner&oldid=113930)"

Contents