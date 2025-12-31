# Component:SnapCircle

> Source: https://wiki.resonite.com/Component:SnapCircle

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SnapCircle&diff=78072) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/da/SnapCircleComponent.png/510px-SnapCircleComponent.png)](https://wiki.resonite.com/File:SnapCircleComponent.png) **Snap Circle** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A snap circle is a component that is able to generate a point on a circle along a plane given a point by another component. Usually this is used in components like the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") to determine where to place the anchors upon clicking (click point is used in such case) When provided a point, it finds the closest point on a circle and normal and returns that to the component that called it.

The functionality of this component is internal, and cannot be used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to snap points using in game code.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the circle should be |
| `Normal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | which direction the circle should face |
| `SnapParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put slots if the component is being used for slot placement. |

Fields
Collapse

## Usage

Used as an anchor point generator in the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") and drawing tools.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapCircle&oldid=78072](https://wiki.resonite.com/index.php?title=Component:SnapCircle&oldid=78072)"

Contents