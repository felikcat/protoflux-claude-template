# Component:SnapSphere

> Source: https://wiki.resonite.com/Component:SnapSphere

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SnapSphere&diff=78067) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/11/SnapSphereComponent.png/510px-SnapSphereComponent.png)](https://wiki.resonite.com/File:SnapSphereComponent.png) **Snap Sphere** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A snap sphere is a component that is able to generate a point in a sphere shape along the outer shell when given a point by another component. Usually this is used in components like the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") to determine where to place the anchors upon clicking (click point is used in such case)

How the snapper determines a point is as such:

1. the snapper component will reduce the distance from the provided point to the center of the snapper to a distance of 1.
2. It then takes the number and aligns it to the closest point on the shape. since this is a sphere snapper, it doesn't need this step.
3. the snapper will then multiply the normalized point by the snapper's size in all 3 axes, and then return the result.

The functionality of this component is internal, and cannot be used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to snap points using in game code.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the radius of the sphere |
| `SnapParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | where the objects to be snapped should go, if they are slots. |

Fields
Collapse

## Usage

Used as an anchor point generator in the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") and drawing tools.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapSphere&oldid=78067](https://wiki.resonite.com/index.php?title=Component:SnapSphere&oldid=78067)"

Contents