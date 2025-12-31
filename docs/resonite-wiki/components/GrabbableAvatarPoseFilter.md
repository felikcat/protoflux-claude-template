# Component:GrabbableAvatarPoseFilter

> Source: https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GrabbableAvatarPoseFilter&diff=93724) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/22/GrabbableAvatarPoseFilterComponent.png/510px-GrabbableAvatarPoseFilterComponent.png)](https://wiki.resonite.com/File:GrabbableAvatarPoseFilterComponent.png) **Grabbable Avatar Pose Filter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabbableAvatarPoseFilter** Component is used to apply pose filters to the user's hand body node that grabbed the [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") on the same Slot this component is on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Filter` | **[IAvatarPoseFilter](https://wiki.resonite.com/Type:IAvatarPoseFilter "Type:IAvatarPoseFilter")** | The filter to apply when a user grabs the [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") this component is on. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Whether this pose filter should be applied before other pose filters currently affecting the user. |

Fields
Collapse

## Usage

This component assigns a Pose Filter to the hand you have grabbed an object on.

This can be used on anything with a [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") component.

## Examples

- [GrabbableAvatarPoseFilter Restrict hand movements when grabbing objects](https://www.youtube.com/watch?v=mTO6zyTOrxI) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

- Component:GrabbableAvatarPoseFilter
- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")
- [Component:ToolAvatarPoseFilter](https://wiki.resonite.com/Component:ToolAvatarPoseFilter "Component:ToolAvatarPoseFilter")
- [Component:AvatarPoseOffset](https://wiki.resonite.com/Component:AvatarPoseOffset "Component:AvatarPoseOffset")
- [Component:AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")
- [Component:AvatarPoseRotationConstraint](https://wiki.resonite.com/Component:AvatarPoseRotationConstraint "Component:AvatarPoseRotationConstraint")
- [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabbableAvatarPoseFilter&oldid=93724](https://wiki.resonite.com/index.php?title=Component:GrabbableAvatarPoseFilter&oldid=93724)"

Contents