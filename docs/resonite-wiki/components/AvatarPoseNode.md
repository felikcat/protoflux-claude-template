# Component:AvatarPoseNode

> Source: https://wiki.resonite.com/Component:AvatarPoseNode

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarPoseNode&diff=93909) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/70/AvatarPoseNodeComponent.png/510px-AvatarPoseNodeComponent.png)](https://wiki.resonite.com/File:AvatarPoseNodeComponent.png) **Avatar Pose Node** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

For detailed information on how this functions for mix and match body parts. Please also see [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars").

The **AvatarPoseNode** component is activated when a user equips an avatar with this component under it. The component drives the transforms of the slot it is on, in order to copy the transforms of an [Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") of the given `Node`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | the node this component is copying. |
| `EquipOrderPriority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority of this node being updated in the list of Pose Nodes on an Avatar. |
| `RunAfterInputUpdate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to run this component's copy Behavior after the engine's input received stage. |
| `MutuallyExclusiveNodes` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") >** | When equipped as part of an avatar, if the user equipping has an [AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") with a [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") value from this list, it is forced to dequip the [Type:IAvatarObjects](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)") bound to it, kicking them off the user. |
| `IsTracking` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is tracking |
| `SourceIsTracking` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the source `_objectSlot` is currently tracking an inputting object like a controller or FBT device |
| `SourceIsActive` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the source `_objectSlot` is active. |
| `SourceIsSimulated` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the source `_objectSlot` is being simulated by the procedural animation system. |
| `_objectSlot` | **[AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** | The object slot this component is getting pose data and tracking data from. |
| `_source` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot of `_objectSlot` |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field to drive to the pose data. Usually the position field of the slot this component is on. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field to drive to the pose data. Usually the rotation field of the slot this component is on. |
| `_scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale to drive to the scale of `_source` if drive scale is enabled on the `_objectSlot`. |
| `_active` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is currently active and setting pose data. |

Fields
Collapse

## Usage

This can be used to make avatars, with only single parts like hands or arms and be mixed and matched with other parts.

## Examples

## See Also

- [Component:AvatarManager](https://wiki.resonite.com/Component:AvatarManager "Component:AvatarManager")
- [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarPoseNode&oldid=93909](https://wiki.resonite.com/index.php?title=Component:AvatarPoseNode&oldid=93909)"

Contents