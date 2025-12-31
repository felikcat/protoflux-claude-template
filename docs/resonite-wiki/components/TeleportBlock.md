# Component:TeleportBlock

> Source: https://wiki.resonite.com/Component:TeleportBlock

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/26/TeleportBlockComponent.png/510px-TeleportBlockComponent.png)](https://wiki.resonite.com/File:TeleportBlockComponent.png) **Teleport Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Teleport Block** component is a component that is used to [Tag](https://wiki.resonite.com/Tag "Tag") colliders like platforms and walls as a place where a user cannot teleport to via the [Teleport Locomotion Mode](https://wiki.resonite.com/Component:TeleportLocomotion "Component:TeleportLocomotion").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Behavior

When a user using teleport mode tries to teleport onto or through a collider with this component, it will make the path turn red and deny them from teleporting to the selected point.

## Examples

Put on walls, and platforms like dangerous areas to prevent teleporting to or through them.

## See Also

- [Teleport Surface](https://wiki.resonite.com/Component:TeleportSurface "Component:TeleportSurface")
- [Teleport Passthrough](https://wiki.resonite.com/Component:TeleportPassthrough "Component:TeleportPassthrough")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TeleportBlock&oldid=98520](https://wiki.resonite.com/index.php?title=Component:TeleportBlock&oldid=98520)"

Contents