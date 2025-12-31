# Component:RemoteConnectionPointDriver

> Source: https://wiki.resonite.com/Component:RemoteConnectionPointDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RemoteConnectionPointDriver&diff=106540) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/56/RemoteConnectionPointDriverComponent.png/510px-RemoteConnectionPointDriverComponent.png)](https://wiki.resonite.com/File:RemoteConnectionPointDriverComponent.png) **Remote Connection Point Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

RemoteConnectionPointDriver allows driving local position, vector, orientation and size from a target Slot. It can be used with [TubeWireMesh](https://wiki.resonite.com/Component:TubeWireMesh "Component:TubeWireMesh") and [StripeWireMesh](https://wiki.resonite.com/Component:StripeWireMesh "Component:StripeWireMesh") to drive the other point from another slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FilterThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The threshold before recalculating the target values. |
| `TargetPoint` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The slot to target. |
| `TargetVector` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The target vector as a local transform under `TargetPoint` |
| `TargetSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The target scale as a local transform offset under `TargetPoint` |
| `TargetOrientation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The target rotation as a local transform offset under `TargetPoint` |
| `LocalPoint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the position of `TargetPoint` with an offset of `TargetVector` converted to this slot's local space. |
| `LocalVector` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with a vector of `TargetVector` in the transform space of `TargetPoint` converted to this slot's local space. |
| `LocalOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the rotation of `TargetPoint` with an offset of `TargetVector` converted to this slot's local space. |
| `LocalSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the scale of `TargetPoint` with an offset of `TargetSize` converted to this slot's local space. |

Fields
Collapse

## Usage

- It's not a complete physical rope simulator or anything, but it lets you connect two endpoints using the different wire mesh types.
- Hyper convenience components that make tube meshes squishy like neurons

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RemoteConnectionPointDriver&oldid=106540](https://wiki.resonite.com/index.php?title=Component:RemoteConnectionPointDriver&oldid=106540)"

Contents