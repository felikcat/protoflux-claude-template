# Component:AvatarPoseSmoothLerp

> Source: https://wiki.resonite.com/Component:AvatarPoseSmoothLerp

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarPoseSmoothLerp&diff=93957) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e5/AvatarPoseSmoothLerpComponent.png/510px-AvatarPoseSmoothLerpComponent.png)](https://wiki.resonite.com/File:AvatarPoseSmoothLerpComponent.png) **AvatarPoseSmoothLerp** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarPoseSmoothLerp** component changes the smoothing speed of the position and rotation of a [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode").

Pose filters are used with components such as the [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter") or [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") in order to restrict movement of any [Type:BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). These components do so by telling the game to apply these pose filters when they interact with said objects. In the case of an Avatar Anchor, this happens while seated. With the grabbable pose filter, this happens when any [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the component on the same Slot is grabbed. This component when used with such components can be used to control placement of a user's hand on an item.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PositionSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast the body node should move. Lower values mean slower speed. |
| `RotationSmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast the body node should rotate. Lower values mean slower speed. |
| `SmoothSimulatedPoses` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this filter should smooth limbs affected by the procedural animation system. |

Fields
Collapse

## Usage

For use with a [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") or a tooltip to smooth the hand movement.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter")
- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")
- [Component:ToolAvatarPoseFilter](https://wiki.resonite.com/Component:ToolAvatarPoseFilter "Component:ToolAvatarPoseFilter")
- [Component:AvatarPoseOffset](https://wiki.resonite.com/Component:AvatarPoseOffset "Component:AvatarPoseOffset")
- Component:AvatarPoseSmoothLerp
- [Component:AvatarPoseRotationConstraint](https://wiki.resonite.com/Component:AvatarPoseRotationConstraint "Component:AvatarPoseRotationConstraint")
- [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarPoseSmoothLerp&oldid=93957](https://wiki.resonite.com/index.php?title=Component:AvatarPoseSmoothLerp&oldid=93957)"

Contents