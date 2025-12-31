# Component:LineTransform

> Source: https://wiki.resonite.com/Component:LineTransform

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2e/LineTransformComponent.png/510px-LineTransformComponent.png)](https://wiki.resonite.com/File:LineTransformComponent.png) **Line Transform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LineTransform** component is a transform driver component used to position an object between two points or slots.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point in local space to transform from. |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point in local space to transform to. |
| `Point0Anchor` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | acts as a slot to offset `Point0` in global space. |
| `Point1Anchor` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | acts as a slot to offset `Point1` in global space. |
| `LinePositionType` | **[PositionType](https://wiki.resonite.com/Type:PositionType "Type:PositionType")** | How to calculate the position on the line using `LinePoint` for the slot this component is on. |
| `PlanePositionType` | **[PositionType](https://wiki.resonite.com/Type:PositionType "Type:PositionType")** | How to calculate the position on the line using `LinePoint` for the slot this component is on. |
| `LinePoint` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where on the line specified by `Point0` and `Point1` in percentage or relative distance that the slot this component is on should be positioned. |
| `OffsetPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset from the point found by `LinePoint` slot this component is on should be. |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation offset from looking along the line. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | drives the target field with the position found by `LinePoint` plus `OffsetPoint` rotated by `RotationOffset` and "looking down the line rotation" around the point found by `LinePoint`. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | drives the target field with `RotationOffset` and "looking down the line rotation" |
| `AllowRepositioning` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow grabbing of the slot this component is on to move the object and change `LinePoint` |
| `RepositionOffset` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether grabbing changes `OffsetPoint` as well. |

Fields
Collapse

## Usage

Can be used to position an object along a track like a slider.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LineTransform&oldid=94861](https://wiki.resonite.com/index.php?title=Component:LineTransform&oldid=94861)"

Contents