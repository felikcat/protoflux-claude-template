# Component:SearchBlock

> Source: https://wiki.resonite.com/Component:SearchBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SearchBlock&diff=98519) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/69/SearchBlockComponent.png/510px-SearchBlockComponent.png)](https://wiki.resonite.com/File:SearchBlockComponent.png) **Search Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Search Block** component, [slots](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component can be used to prevent either:

- A user from grabbing an item from contacting certain colliders.
- A user from equipping an avatar when clicking on a limb or collider attached to it.
- A user from equipping a tool tip by clicking on a certain part of it.
- A user from clicking a physical button when clicking on a collider parented to the physical button further down the hierarchy, or any button type not just physical buttons.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

## Examples

Example Panel made by [Ukilop](https://wiki.resonite.com/index.php?title=User:Ukilop&action=edit&redlink=1 "User:Ukilop (page does not exist)") of how the component works.

[![](https://wiki.resonite.com/images/thumb/c/c2/SearchBlockExample.png/500px-SearchBlockExample.png)](https://wiki.resonite.com/File:SearchBlockExample.png)

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SearchBlock&oldid=98519](https://wiki.resonite.com/index.php?title=Component:SearchBlock&oldid=98519)"

Contents