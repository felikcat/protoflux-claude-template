# Component:AvatarObjectSlot

> Source: https://wiki.resonite.com/Component:AvatarObjectSlot

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarObjectSlot&diff=93911) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dd/AvatarObjectSlotComponent.png/510px-AvatarObjectSlotComponent.png)](https://wiki.resonite.com/File:AvatarObjectSlotComponent.png) **AvatarObjectSlot** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

For detailed information on how this functions for mix and match body parts. Please also see [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars").

Avatar Object slot is a component that is used to move and drive certain parts of the avatar like the head and hand body parts.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Whether to do the equip checking on this AvatarObjectSlot before other AvatarObjectSlots |
| `Equipped` | _direct_ **[LinkRef\`1](https://wiki.resonite.com/index.php?title=Type:LinkRef%601&action=edit&redlink=1 "Type:LinkRef`1 (page does not exist)") < [IAvatarObject](https://wiki.resonite.com/index.php?title=Type:IAvatarObject&action=edit&redlink=1 "Type:IAvatarObject (page does not exist)") >** | Usually an [Avatar Pose Node](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode") that is on one of the proxies on an avatar. |
| `Node` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | the body node of the avatar this component's slot is. Unless already specified by a [Biped Rig Component](https://wiki.resonite.com/Component:BipedRig "Component:BipedRig") higher up in the hierarchy. |
| `IsTracking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is currently being simulated by the procedural animation system. |
| `IsActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is currently active and controlling an avatar. |
| `IsSimulated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this object slot is being controlled by the procedural animation system. |
| `DriveActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to drive the active of this slot when hooked into by an [Avatar Pose Node](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode"). |
| `DriveScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to drive the scale of this slot when hooked into by an [Avatar Pose Node](https://wiki.resonite.com/Component:AvatarPoseNode "Component:AvatarPoseNode"). |
| `DoNotSimulate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not control this with the procedural locomotion system |
| `Filters` | _direct_ **[PrioritySyncRefList\`1](https://wiki.resonite.com/index.php?title=Type:PrioritySyncRefList%601&action=edit&redlink=1 "Type:PrioritySyncRefList`1 (page does not exist)") < [IAvatarPoseFilter](https://wiki.resonite.com/Type:IAvatarPoseFilter "Type:IAvatarPoseFilter") >** | Filters that are currently effecting this and their priorities. See [Avatar Pose Filters](https://wiki.resonite.com/Category:Components:Users:Common_Avatar_System:Pose_Filters "Category:Components:Users:Common Avatar System:Pose Filters") |
| `_autoSmoothing` | **[AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")** | The Component currently smoothing the transform changes of this Avatar Object slot. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarObjectSlot&oldid=93911](https://wiki.resonite.com/index.php?title=Component:AvatarObjectSlot&oldid=93911)"

Contents