# Component:RaycastDriver

> Source: https://wiki.resonite.com/Component:RaycastDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RaycastDriver&diff=97697) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/88/RaycastDriverComponent.png/510px-RaycastDriverComponent.png)](https://wiki.resonite.com/File:RaycastDriverComponent.png) **RaycastDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RaycastDriver** component drives the position of the [Slot](https://wiki.resonite.com/Slot "Slot") it is attached to to the location of the hit point of a raycast and aligns its rotation to the normal of the hit object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IgnoreHierarchy` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | a hiearchy of slots which to ignore the colliders for |
| `FilterDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | ignore hit detections before this distance. |
| `Origin` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to start the raycast from. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset from `Origin` before starting the raycast. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction in `Origin`'s local space to shoot in. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum distance to raycast for. |
| `NoHitDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far to raycast shoot for in meters till reporting no hit. |
| `Filter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | A [sync delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") that takes a collider and returns a bool. if a collider returns false from this sync delegate, it is ignored when raycasting for objects. |
| `_positionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field to drive. This does not actually affect the field that is driven, but if it is not filled, the component will not function. |
| `_rotationDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field to drive. This does not actually affect the field that is driven, but if it is not filled, the rotation of the slot is not changed. Aligns itself to the normal of the surface this raycast hit, or `(0,0,0)`. |

Fields
Collapse

## Usage

When placed on a slot, `_positionDrive` and `_rotationDrive` are automatically filled to the slot's position and rotation. These fields are not actually effective, as this component always writes to the position/rotation of the slot it is on. However, if either of these fields are omitted, the respective functionality of the raycast is not performed.

The raycast is constructed in the [local coordinate space](https://wiki.resonite.com/Local_coordinate_space "Local coordinate space") of `Origin`, where `Offset` controls the origin of the ray relative to the origin and `Direction` controls the direction of the ray relative to the origin.

`MaxDistance` controls the maximum distance that the raycast will travel. If a raycast is unable to make contact with a collider within this distance, the position of the slot will be set to `NoHitDistance` in the direction of the raycast. **These two distances are in global scale**, and are _not_ affected by either the slot's local scale or the scale of the `Origin` slot.

If the ray hits a collider, the rotation of the slot will be aligned to the normal of the hit point. This rotation can be transformed into the normal vector by using the [Get Forward](https://wiki.resonite.com/ProtoFlux:Get_Forward "ProtoFlux:Get Forward") node on the RaycastDriver slot. If the raycast does not hit a collider, the rotation will be set to `(0, 0, 0)`.

### Filtering

There are two ways of filtering what colliders the raycast is able to make contact with.

If `IgnoreHierarchy` is filled, the raycast will ignore all colliders present under the provided hierarchy. This can be useful if one needs to ignore, for example, the object that the raycast originates from, the active user if part of a tool, or only the local user of a raycast originating from all users locally.

The `Filter` field is much more flexible. It takes a [`System.Func<ICollider, bool>`](https://learn.microsoft.com/en-us/dotnet/api/system.func-2) where `ICollider` is the potentially hit collider, and `bool` is the return value of the function. If the bool is true, the raycast will consider the collider hit. Else, the raycast will ignore the collider.

As of the time of writing, the `Filter` field is unable to be directly controlled by users with custom functions. There currently exists one singular function, `FilterUsers`, that is able to be put in this field. This function can be retrieved by using a [meter tool](https://wiki.resonite.com/Meter_tool "Meter tool") set to `Perpendicular`, inspecting the resulting point, and grabbing the function off the resulting RaycastDriver. This function filters out every single user in the session from being hit by the raycast, which can be useful in specific cases.

## Examples

Can be used to place objects onto a floor, or as a laser pointer, or as part of a draw on a surface pen.

## See Also

- The lighter version, [RayDriver](https://wiki.resonite.com/Component:RayDriver "Component:RayDriver")
- [ProtoFlux:Raycaster](https://wiki.resonite.com/ProtoFlux:Raycaster "ProtoFlux:Raycaster")
- [ProtoFlux:Raycast One](https://wiki.resonite.com/ProtoFlux:Raycast_One "ProtoFlux:Raycast One")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RaycastDriver&oldid=97697](https://wiki.resonite.com/index.php?title=Component:RaycastDriver&oldid=97697)"

Contents