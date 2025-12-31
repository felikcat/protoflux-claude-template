# Component:TeleportSurface

> Source: https://wiki.resonite.com/Component:TeleportSurface

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TeleportSurface&diff=98522) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/63/TeleportSurfaceComponent.png/510px-TeleportSurfaceComponent.png)](https://wiki.resonite.com/File:TeleportSurfaceComponent.png) **Teleport Surface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The **Teleport Surface** component is a component that is used to mark surfaces on [slots](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component in a world as specific spots the user can teleport to via the [Teleport Locomotion Mode](https://wiki.resonite.com/Component:TeleportLocomotion "Component:TeleportLocomotion") regardless of the CharacterCollider field on a slot's collider.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Attach this component to the same slot as a collider to mark that collider as a spot a user can specifically teleport to.

## Examples

This can be used along with [Teleport Block](https://wiki.resonite.com/Component:TeleportBlock "Component:TeleportBlock") to make a maze that can only be navigated via teleporting.

## Related Components

- [Teleport Passthrough](https://wiki.resonite.com/Component:TeleportPassthrough "Component:TeleportPassthrough")
- [Teleport Block](https://wiki.resonite.com/Component:TeleportBlock "Component:TeleportBlock")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TeleportSurface&oldid=98522](https://wiki.resonite.com/index.php?title=Component:TeleportSurface&oldid=98522)"

Contents