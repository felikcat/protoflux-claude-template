# Component:LocomotionAnimationColliderBlock

> Source: https://wiki.resonite.com/Component:LocomotionAnimationColliderBlock

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8a/LocomotionAnimationColliderBlockComponent.png/510px-LocomotionAnimationColliderBlockComponent.png)](https://wiki.resonite.com/File:LocomotionAnimationColliderBlockComponent.png) **Locomotion Animation Collider Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component can be used in combination with the [LocomotionAnimationBodyCollider](https://wiki.resonite.com/Component:LocomotionAnimationBodyCollider "Component:LocomotionAnimationBodyCollider") component to control which colliders on an avatar should be avoided by the avatar's hands.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Add this component to the top of a hierarchy of any colliders on your avatar that you don't want your hands colliding with. This component can also be added to environment colliders if you want feet collisions to ignore them.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:LocomotionAnimationBodyCollider](https://wiki.resonite.com/Component:LocomotionAnimationBodyCollider "Component:LocomotionAnimationBodyCollider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationColliderBlock&oldid=97602](https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationColliderBlock&oldid=97602)"

Contents