# Component:AxisPanner

> Source: https://wiki.resonite.com/Component:AxisPanner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AxisPanner&diff=93902) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/AxisPannerComponent.png/510px-AxisPannerComponent.png)](https://wiki.resonite.com/File:AxisPannerComponent.png) **Axis Panner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisPanner** component is used to move an object along a single axis linearly. This component can affect position and scale.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TimeBase` | **[IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Double](https://wiki.resonite.com/Type:Double "Type:Double") >** | Reference to the timebase or "clock" that the component will use for moving an object. Possible components that can be used as an input include [AuthorityTimeBase](https://wiki.resonite.com/Component:AuthorityTimeBase "Component:AuthorityTimeBase"). |
| `Speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed at which the object will move. |
| `Range` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the object will move. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Where the object starts its move. |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction that the object will move in. |
| `ReferenceScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Sets the maximum scale that the object will become at the halfway point. Starting at 0 the object will grow to this size and then back to 0. |
| `FullScaleRangeRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Changes the duration that the object scale will remain at the ReferenceScale size. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Reference to the position that is being driven. By default, set the to object that this component is first attached to. |
| `_scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Reference to the scale that is being driven. By default, set to null. |

Fields
Collapse

## Usage

## Examples

- [AxisPanner tutorial](https://www.youtube.com/watch?v=k7Q89GWGDAk) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisPanner&oldid=93902](https://wiki.resonite.com/index.php?title=Component:AxisPanner&oldid=93902)"

Contents