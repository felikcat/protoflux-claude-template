# Component:ButtonPressEventRelay

> Source: https://wiki.resonite.com/Component:ButtonPressEventRelay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonPressEventRelay&diff=92316) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/80/ButtonPressEventRelayComponent.png/510px-ButtonPressEventRelayComponent.png)](https://wiki.resonite.com/File:ButtonPressEventRelayComponent.png) **Button Press Event Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonPressEventRelay** component takes in a [slot](https://wiki.resonite.com/Slot "Slot") target, and if any [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") press event happens with this component on a slot, will also send a signal to that target slot, and the components on that target slot will trigger with press events (if applicable).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The [slot](https://wiki.resonite.com/Slot "Slot") to send the signal to. |

Fields
Collapse

## Usage

Useful for sending multiple signals from one press event.

## Examples

## See Also

- Component:ButtonPressEventRelay
- [Component:ButtonHoverEventRelay](https://wiki.resonite.com/Component:ButtonHoverEventRelay "Component:ButtonHoverEventRelay")
- [Component:ButtonRelay](https://wiki.resonite.com/Component:ButtonRelay "Component:ButtonRelay")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonPressEventRelay&oldid=92316](https://wiki.resonite.com/index.php?title=Component:ButtonPressEventRelay&oldid=92316)"

Contents