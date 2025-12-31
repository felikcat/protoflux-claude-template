# Component:TouchEventRelay

> Source: https://wiki.resonite.com/Component:TouchEventRelay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TouchEventRelay&diff=106593) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/f/f5/TouchEventRelayComponent.png)](https://wiki.resonite.com/File:TouchEventRelayComponent.png) **Touch Event Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchEventRelay** component is used to relay touch events recieved by a slot to other ITouchables.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Touched` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | The sync delegate to call when this receives a touch event. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows touch events from a user not looking directly at the slot with this component. |
| `TouchableTargets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[ITouchable](https://wiki.resonite.com/Type:ITouchable "Type:ITouchable")** | Target touchable components to send the touch event to. |

Fields
Collapse

## Usage

- To trigger a hyperlink component without a touchable/interactable component you can use a TouchEventRelay. You a touch event relay on the collider of your object, then put a hyperlink or other touchables as children (with no colliders on them) then add them to the TouchableTargets list of the TouchEventRelay.

## Examples

- [Using TouchEventRelay for complicated Touch Events](https://www.youtube.com/watch?v=5n2veHi-CJU) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

- [Touchable Events](https://wiki.resonite.com/ProtoFlux:Touchable_Events "ProtoFlux:Touchable Events") can be used with TouchEventRelay.

TouchEventRelay can relay events from a Touchable element to fire another ITouchable component.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchEventRelay&oldid=106593](https://wiki.resonite.com/index.php?title=Component:TouchEventRelay&oldid=106593)"

Contents