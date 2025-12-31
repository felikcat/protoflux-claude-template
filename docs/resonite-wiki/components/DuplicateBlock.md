# Component:DuplicateBlock

> Source: https://wiki.resonite.com/Component:DuplicateBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DuplicateBlock&diff=98516) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b4/DuplicateBlockComponent.png/510px-DuplicateBlockComponent.png)](https://wiki.resonite.com/File:DuplicateBlockComponent.png) **Duplicate Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Duplicate Block** component blocks duplication of a [Grabbable](https://wiki.resonite.com/Grabbable_(Component) "Grabbable (Component)") [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component by using the [Context menu](https://wiki.resonite.com/Context_menu "Context menu"), but not via the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") or [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

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

Can be used to prevent users from duplicating cards during a card game, or for other key items that need to stay unique.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DuplicateBlock&oldid=98516](https://wiki.resonite.com/index.php?title=Component:DuplicateBlock&oldid=98516)"

Contents