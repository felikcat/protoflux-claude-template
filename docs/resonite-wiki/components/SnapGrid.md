# Component:SnapGrid

> Source: https://wiki.resonite.com/Component:SnapGrid

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SnapGrid&diff=91552) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/be/SnapGridComponent.png/510px-SnapGridComponent.png)](https://wiki.resonite.com/File:SnapGridComponent.png) **Snap Grid** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A snap grid is a component that is able to generate a point in a grid of points given a point by another component. Usually this is used in components like the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") to determine where to place the anchors upon clicking (click point is used in such case). Since this generates a grid of points, it takes the inserted point and rounds it to the nearest grid point, then returns it to the component that called it.

The functionality of this component is internal, and cannot be used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to snap points using in game code.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BoundsSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big the grid is in total, and determines the total size available for grid points to take up |
| `GridSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big each grid point is, or in other words, how far apart they are. |
| `ColliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `SnapParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put slots if the component is being used for slot placement. |

Fields
Collapse

## Usage

Used as an anchor point generator in the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") and drawing tools.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapGrid&oldid=91552](https://wiki.resonite.com/index.php?title=Component:SnapGrid&oldid=91552)"

Contents