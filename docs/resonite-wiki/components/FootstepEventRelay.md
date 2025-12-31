# Component:FootstepEventRelay

> Source: https://wiki.resonite.com/Component:FootstepEventRelay

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8e/FootstepEventRelayComponent.png/510px-FootstepEventRelayComponent.png)](https://wiki.resonite.com/File:FootstepEventRelayComponent.png) **Footstep Event Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FootstepEventRelay** component can be put on a user's feet or an object with a collider to receive footstep events. The events are then sent to another slot or any number of [ProtoFlux:FootstepEvents](https://wiki.resonite.com/ProtoFlux:FootstepEvents "ProtoFlux:FootstepEvents") ProtoFlux nodes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to relay footstep events to. |

Fields
Collapse

## Usage

Used to receive and relay footstep events.

## Examples

Can be used with ProtoFlux to make personal footstep sounds, or trigger other events as the user walks.

The world "Ripple Ripple Particle" by [orange](https://wiki.resonite.com/User:Orange "User:Orange") uses this for its effects.

## See Also

[ProtoFlux:FootstepEvents](https://wiki.resonite.com/ProtoFlux:FootstepEvents "ProtoFlux:FootstepEvents")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FootstepEventRelay&oldid=112865](https://wiki.resonite.com/index.php?title=Component:FootstepEventRelay&oldid=112865)"

Contents