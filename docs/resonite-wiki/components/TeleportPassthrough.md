# Component:TeleportPassthrough

> Source: https://wiki.resonite.com/Component:TeleportPassthrough

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TeleportPassthrough&diff=98521) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3a/TeleportPassthroughComponent.png/510px-TeleportPassthroughComponent.png)](https://wiki.resonite.com/File:TeleportPassthroughComponent.png) **Teleport Passthrough** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Teleport Passthrough** component makes a collider on the same [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component act as if the collider doesn't exist to the teleport selector when teleporting via the [Teleport Locomotion Mode](https://wiki.resonite.com/Component:TeleportLocomotion "Component:TeleportLocomotion").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Attach to a slot with a collider, to enable teleporting through a wall via the [Teleport Locomotion Mode](https://wiki.resonite.com/Component:TeleportLocomotion "Component:TeleportLocomotion").

## Examples

This can be used in puzzle rooms where the way out or forward in a puzzle is by teleporting.

## Related Components

- [Teleport Surface](https://wiki.resonite.com/Component:TeleportSurface "Component:TeleportSurface")
- [Teleport Block](https://wiki.resonite.com/Component:TeleportBlock "Component:TeleportBlock")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TeleportPassthrough&oldid=98521](https://wiki.resonite.com/index.php?title=Component:TeleportPassthrough&oldid=98521)"

Contents