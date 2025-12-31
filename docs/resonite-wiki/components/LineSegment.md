# Component:LineSegment

> Source: https://wiki.resonite.com/Component:LineSegment

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/LineSegmentComponent.png/510px-LineSegmentComponent.png)](https://wiki.resonite.com/File:LineSegmentComponent.png) **Line Segment** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Line Segment** component is used to create a line between two slots or two local points in space.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the generated line |
| `Sides` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sides along the radius circle this cylinder should have. |
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Point 1 as a number in local space to place point 1 of the line visual. |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Point 2 as a number in local space to place point 2 of the line visual. |
| `Anchor0` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | Point 1 as a slot to place point 1 of the line visual. |
| `Anchor1` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | Point 2 as a slot to place point 2 of the line visual. |
| `_cylinder` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[CylinderMesh](https://wiki.resonite.com/Component:CylinderMesh "Component:CylinderMesh")** | The line visual to control. |
| `_collider` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[CylinderCollider](https://wiki.resonite.com/Component:CylinderCollider "Component:CylinderCollider")** | The collider for the line visual. |
| `_offset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the position of the visual + collider slot. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the rotation of the visual + collider slot. |
| `_visualScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the scale of the visual + collider slot. |

Fields
Collapse

## Usage

Can be used to make a line that connects two points. To use an abitrary point, one can use [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") or [Spatial Variables](https://wiki.resonite.com/Spatial_Variables "Spatial Variables") in order to dynamically set `Anchor0` and/or `Anchor1` using code or proximity.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LineSegment&oldid=103809](https://wiki.resonite.com/index.php?title=Component:LineSegment&oldid=103809)"

Contents