# Component:CircleAligner

> Source: https://wiki.resonite.com/Component:CircleAligner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CircleAligner&diff=97438) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2f/CircleAlignerComponent.png/510px-CircleAlignerComponent.png)](https://wiki.resonite.com/File:CircleAlignerComponent.png) **Circle Aligner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CircleAligner** component is used to position a list of slots in a circle.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoAddChildren` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether slots below this component's slot in the hierarchy are automatically added to `Items` |
| `AutoAddIgnoreTags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | If a slot has a Tag matching one of the tags in this list, it will not be auto added to `Items` |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis around which the slots will be aligned. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the circle that the slots will be positioned on. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Offsets the starting position of the circle. |
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | 360 by default. If smaller, the slots will only fill that section of a circle. Likewise, if it is larger than 360, the slots will wrap around the circle multiple times. |
| `FillWholeArc` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, the last slot will be at the very end of the arch, otherwise there will be a gap after the last slots. |
| `RotationOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | An offset, in degrees, that is applied to the rotation of the target slots. |
| `Items` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[CircleAligner.Item](https://wiki.resonite.com/Component:CircleAligner#Item)** | The list of slots to be aligned. |

Fields
Collapse

## Item

| Name | Type | Description |
| --- | --- | --- |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to align. |
| `AngleOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset amount of degrees the object should rotate from the default of pointing towards the center. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of `Root`. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Rotation field of `Root`. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

- [CircleAligner tutorial](https://www.youtube.com/watch?v=5nX-eb9p9s4) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CircleAligner&oldid=97438](https://wiki.resonite.com/index.php?title=Component:CircleAligner&oldid=97438)"

Contents