# Component:LocomotionAnimationBodyCollider

> Source: https://wiki.resonite.com/Component:LocomotionAnimationBodyCollider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/23/LocomotionAnimationBodyColliderComponent.png/510px-LocomotionAnimationBodyColliderComponent.png)](https://wiki.resonite.com/File:LocomotionAnimationBodyColliderComponent.png) **Locomotion Animation Body Collider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocomotionAnimationBodyCollider** component is required for any colliders to be considered for self-collision for the hands.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IgnoreForLeftHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this collider is ignored by the player's left hand during locomotion. |
| `IgnoreForRightHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this collider is ignored by the player's right hand during locomotion. |

Fields
Collapse

## Usage

Attach to a slot on an avatar with a collider. That collider will now be a collider the hands will hit and go around while the user is walking in desktop.

## Examples

Can be used on avatars with bigger thighs, or to avoid a bigger chest area.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationBodyCollider&oldid=94879](https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationBodyCollider&oldid=94879)"

Contents