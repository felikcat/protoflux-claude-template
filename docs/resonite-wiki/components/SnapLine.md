# Component:SnapLine

> Source: https://wiki.resonite.com/Component:SnapLine

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SnapLine&diff=78070) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d2/SnapLineComponent.png/510px-SnapLineComponent.png)](https://wiki.resonite.com/File:SnapLineComponent.png) **Snap Line** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A snap line is a component that is able to generate a point in a line given a point by another component. Usually this is used in components like the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") to determine where to place the anchors upon clicking (click point is used in such case) When provided a point, it finds the closest point on a line and returns that to the component that called it.

The functionality of this component is internal, and cannot be used by [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to snap points using in game code.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The first point to use to define the line |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the second point to define the line |
| `Anchor0` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | an override to use instead of Point0 to define the line |
| `Anchor1` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | an override to use instead of Point1 to define the line |
| `SnapParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to put slots if the component is being used for slot placement. |

Fields
Collapse

## Usage

Used as an anchor point generator in the [Multi User Avatar Anchor Component](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor") and drawing tools.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapLine&oldid=78070](https://wiki.resonite.com/index.php?title=Component:SnapLine&oldid=78070)"

Contents