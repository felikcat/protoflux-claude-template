# Component:AvatarPoseBoxConstraint

> Source: https://wiki.resonite.com/Component:AvatarPoseBoxConstraint

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarPoseBoxConstraint&diff=93723) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b2/AvatarPoseBoxConstraintComponent.png/510px-AvatarPoseBoxConstraintComponent.png)](https://wiki.resonite.com/File:AvatarPoseBoxConstraintComponent.png) **Avatar Pose Box Constraint** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarPoseBoxConstraint** component is a BodyPoseFilter that can be used in the construction of tool tips, anchors, grabbable items, and more. This pose filter is used to force the slot corresponding to a body node (In the case of a hand for example, it will constrict the position of the hand bone position, rather than the whole hand) to stay within a rotatable box specified.

Pose filters are used with components such as the [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter") or [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") in order to restrict movement of any [Type:BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). These components do so by telling the game to apply these pose filters when they interact with said objects. In the case of an Avatar Anchor, this happens while seated. With the grabbable pose filter, this happens when any [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the component on the same Slot is grabbed. This component when used with such components can be used to control placement of a user's hand on an item.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BoxSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the size of the box that a user's body node should be constrained within. (0,0,0) is valid for this field. |
| `DefaultPoseReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot which the box will be positioned, rotated, and scaled by. If null, this is the slot this component is on. |
| `ProcessSimulatedPoses` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to affect simulated poses like from the animation system. |

Fields
Collapse

## Usage

This is widely used in seats where the user's legs and hips are posed in a sitting position, like when sitting in a car.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter")
- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")
- [Component:ToolAvatarPoseFilter](https://wiki.resonite.com/Component:ToolAvatarPoseFilter "Component:ToolAvatarPoseFilter")
- [Component:AvatarPoseOffset](https://wiki.resonite.com/Component:AvatarPoseOffset "Component:AvatarPoseOffset")
- [Component:AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")
- [Component:AvatarPoseRotationConstraint](https://wiki.resonite.com/Component:AvatarPoseRotationConstraint "Component:AvatarPoseRotationConstraint")
- Component:AvatarPoseBoxConstraint

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarPoseBoxConstraint&oldid=93723](https://wiki.resonite.com/index.php?title=Component:AvatarPoseBoxConstraint&oldid=93723)"

Contents