# Component:SnapPlane

> Source: https://wiki.resonite.com/Component:SnapPlane

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SnapPlane&diff=78069) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/10/SnapPlaneComponent.png/510px-SnapPlaneComponent.png)](https://wiki.resonite.com/File:SnapPlaneComponent.png) **Snap Plane** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A snap plane is a component that is able to generate a point in a plane shape when given a point by another component. Usually this is used in components like the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") to determine where to place the anchors upon clicking (click point is used in such case). This component will take a given point by another component and find the closest surface point to a plane with a normal + with a center positioned at the slot it is on. This component will then return the point to the component that called it.

The functionality of this component is internal, and cannot be used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to snap points using in game code.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Normal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Determines which direction the plane is facing |
| `SnapParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put slots if the component is being used for slot placement. |

Fields
Collapse

## Usage

Used as an anchor point generator in the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") and drawing tools.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapPlane&oldid=78069](https://wiki.resonite.com/index.php?title=Component:SnapPlane&oldid=78069)"

Contents