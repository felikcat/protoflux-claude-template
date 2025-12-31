# Component:AvatarPoseRotationConstraint

> Source: https://wiki.resonite.com/Component:AvatarPoseRotationConstraint

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarPoseRotationConstraint&diff=93728) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5f/AvatarPoseRotationConstraintComponent.png/510px-AvatarPoseRotationConstraintComponent.png)](https://wiki.resonite.com/File:AvatarPoseRotationConstraintComponent.png) **AvatarPoseRotationConstraint** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarPoseRotationConstraint** component is used to either restrict the rotation direction of the user's arm when using a tooltip, or to restrict the rotation of a particular [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode").

Pose filters are used with components such as the [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter") or [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") in order to restrict movement of any [Type:BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). These components do so by telling the game to apply these pose filters when they interact with said objects. In the case of an Avatar Anchor, this happens while seated. With the grabbable pose filter, this happens when any [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the component on the same Slot is grabbed. This component when used with such components can be used to control placement of a user's hand on an item.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MaxTwist` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the max twist in degrees allowed for the object being filtered. |
| `MaxSwing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the max swing in degrees allowed for the object being filtered. |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | swing axis direction for the object being filtered. |
| `TwistReferenceAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The twist axis direction for the object being filtered. |

Fields
Collapse

## Usage

Used in avatar anchors and in tooltip contraints.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter")
- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")
- [Component:ToolAvatarPoseFilter](https://wiki.resonite.com/Component:ToolAvatarPoseFilter "Component:ToolAvatarPoseFilter")
- [Component:AvatarPoseOffset](https://wiki.resonite.com/Component:AvatarPoseOffset "Component:AvatarPoseOffset")
- [Component:AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")
- Component:AvatarPoseRotationConstraint
- [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarPoseRotationConstraint&oldid=93728](https://wiki.resonite.com/index.php?title=Component:AvatarPoseRotationConstraint&oldid=93728)"

Contents