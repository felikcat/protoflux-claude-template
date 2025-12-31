# Component:ButtonDelegateRelay

> Source: https://wiki.resonite.com/Component:ButtonDelegateRelay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonDelegateRelay&diff=92314) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/ButtonDelegateRelay%601Component.png/510px-ButtonDelegateRelay%601Component.png)](https://wiki.resonite.com/File:ButtonDelegateRelay%601Component.png) **Button Delegate Relay\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonDelegateRelay** component sends a signal to a button event handler (usually something internal like a [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate")).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DoublePressDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how long it takes before it is to late to count as a double press. |
| `ReleasePressInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of time it takes to release the button. |
| `Argument` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **T** | The sync Delegate reference. |
| `ButtonPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") <T>** | The place to send the signal. |

Fields
Collapse

## Usage

This can send a signal internally.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonDelegateRelay&oldid=92314](https://wiki.resonite.com/index.php?title=Component:ButtonDelegateRelay&oldid=92314)"

Contents