# Component:NoDestroyUndo

> Source: https://wiki.resonite.com/Component:NoDestroyUndo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:NoDestroyUndo&diff=105212) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0f/NoDestroyUndoComponent.png/510px-NoDestroyUndoComponent.png)](https://wiki.resonite.com/File:NoDestroyUndoComponent.png) **No Destroy Undo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NoDestroyUndo** component prevents an [Undo](https://wiki.resonite.com/Undo "Undo") step from being created when destroying the slot that the component is attached to.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component is currently non-functional and using it will have no effect. see issue [#979](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/979).


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Attach to the root slot that will be destroyed. this will prevent the slot from being brought back through undoing after it is destroyed.

## Examples

Useful for objects that should be one of a kind, or other implementations.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NoDestroyUndo&oldid=105212](https://wiki.resonite.com/index.php?title=Component:NoDestroyUndo&oldid=105212)"

Contents