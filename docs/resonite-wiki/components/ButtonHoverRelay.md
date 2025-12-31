# Component:ButtonHoverRelay

> Source: https://wiki.resonite.com/Component:ButtonHoverRelay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonHoverRelay&diff=90415) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/20/ButtonHoverRelayComponent.png/510px-ButtonHoverRelayComponent.png)](https://wiki.resonite.com/File:ButtonHoverRelayComponent.png) **Button Hover Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonHoverRelay** component sends a signal to a button event handler (usually something internal like a [Method Proxy](https://wiki.resonite.com/ProtoFlux:Method_Proxy "ProtoFlux:Method Proxy")).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OnHoverEnter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Sends a signal when hovering begins. |
| `OnHoverStay` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Sends a signal when hovering. |
| `OnHoverLeave` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | Sends a signal when hovering ends. |

Fields
Collapse

## Usage

This can send a signal internally.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonHoverRelay&oldid=90415](https://wiki.resonite.com/index.php?title=Component:ButtonHoverRelay&oldid=90415)"

Contents