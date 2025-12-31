# Component:AvatarPoseOffset

> Source: https://wiki.resonite.com/Component:AvatarPoseOffset

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarPoseOffset&diff=102388) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/79/AvatarPoseOffsetComponent.png/510px-AvatarPoseOffsetComponent.png)](https://wiki.resonite.com/File:AvatarPoseOffsetComponent.png) **AvatarPoseOffset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Avatar Pose Offset Component is used to offset a user's limb while they use a tool tip or sit in an anchor.

Pose filters are used with components such as the [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter") or [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") in order to restrict movement of any [Type:BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). These components do so by telling the game to apply these pose filters when they interact with said objects. In the case of an Avatar Anchor, this happens while seated. With the grabbable pose filter, this happens when any [Type:IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the component on the same Slot is grabbed. This component when used with such components can be used to control placement of a user's hand on an item.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PositionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much position to offset a body node by after previous pose constraints have been applied. |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much rotation to offset a body node by after previous pose constraints have been applied. |

Fields
Collapse

## Usage

this can be applied in a certain order relative to other constraints in [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") or in use with a tooltip. Because of this, the Component can be used to either make a user's hand(s) or feet positioned as an offset to where they originally are tracked or to apply an offset after another Pose component has restricted movement.

This component's rotation can be driven in combination with using a [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint") to freeze the user's body node. this is done by driving `RotationOffset` to counteract the rotation of the user's hand, effectively offsetting it back to zero and stopping movement.

## Examples

This is used extensively in [989onan's](https://wiki.resonite.com/User:989onan "User:989onan") MMD player, where the hands are first constrained by other pose components and then their rotation offset by this component.

## See Also

- [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter")
- [Component:AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")
- [Component:ToolAvatarPoseFilter](https://wiki.resonite.com/Component:ToolAvatarPoseFilter "Component:ToolAvatarPoseFilter")
- Component:AvatarPoseOffset
- [Component:AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")
- [Component:AvatarPoseRotationConstraint](https://wiki.resonite.com/Component:AvatarPoseRotationConstraint "Component:AvatarPoseRotationConstraint")
- [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarPoseOffset&oldid=102388](https://wiki.resonite.com/index.php?title=Component:AvatarPoseOffset&oldid=102388)"

Contents