# Component:SnapPoint

> Source: https://wiki.resonite.com/Component:SnapPoint

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SnapPoint&diff=78068) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/SnapPointComponent.png/510px-SnapPointComponent.png)](https://wiki.resonite.com/File:SnapPointComponent.png) **Snap Point** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A snap point is a component that when called by another component always returns the point of the slot it is on (0,0,0). Usually this is used in components like the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") to determine where to place the anchors upon clicking (click point is used in such case). This component will take a given point by another component and return the position the slot is on, acting as a nullifier of incoming data.

The functionality of this component is internal, and cannot be used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to snap points using in game code.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SnapParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put slots if the component is being used for slot placement. |

Fields
Collapse

## Usage

Used as an anchor point generator in the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") and drawing tools.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapPoint&oldid=78068](https://wiki.resonite.com/index.php?title=Component:SnapPoint&oldid=78068)"

Contents