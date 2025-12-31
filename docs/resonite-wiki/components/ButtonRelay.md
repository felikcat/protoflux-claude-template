# Component:ButtonRelay

> Source: https://wiki.resonite.com/Component:ButtonRelay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonRelay&diff=98198) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/21/ButtonRelayComponent.png/510px-ButtonRelayComponent.png)](https://wiki.resonite.com/File:ButtonRelayComponent.png) **Button Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonRelay** component sends a signal (and optionally with a [Value Type](https://wiki.resonite.com/Value_Type "Value Type")) to a button event handler (usually something internal like a [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate")).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DoublePressDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how long it takes before it is to late to count as a double press. |
| `ReleasePressInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of time it takes to release the button. |
| `ButtonPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The place to send the signal. |

Fields
Collapse

## Usage

This can send a signal internally.

## Examples

## See Also

- [Component:ButtonPressEventRelay](https://wiki.resonite.com/Component:ButtonPressEventRelay "Component:ButtonPressEventRelay")
- [Component:ButtonHoverEventRelay](https://wiki.resonite.com/Component:ButtonHoverEventRelay "Component:ButtonHoverEventRelay")
- Component:ButtonRelay

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonRelay&oldid=98198](https://wiki.resonite.com/index.php?title=Component:ButtonRelay&oldid=98198)"

Contents