# Component:ArcLayout

> Source: https://wiki.resonite.com/Component:ArcLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ArcLayout&diff=97378) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/45/ArcLayoutComponent.png/510px-ArcLayoutComponent.png)](https://wiki.resonite.com/File:ArcLayoutComponent.png) **ArcLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ArcLayout** is a component primarily used in a [user's](https://wiki.resonite.com/User "User") [context menu](https://wiki.resonite.com/Context_menu "Context menu"). It requires a set of [slots](https://wiki.resonite.com/Slot "Slot") under the slot the component is attached to, and each slot needs an [OutlinedArc Component](https://wiki.resonite.com/Component:OutlinedArc "Component:OutlinedArc") and an [ArcSegmentLayout Component](https://wiki.resonite.com/Component:ArcSegmentLayout "Component:ArcSegmentLayout").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of the circle in degrees to cover with the arc elements. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the amount to rotate the arc elements around the center in degrees from the default position. |
| `Separation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to separate the elements from each other. |
| `CenterAtSeparation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Centers the separation point of this layout. |
| `ProportionalSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Keep all segments of the arc proportional in size. |
| `ItemDirection` | **[ArcLayout.Direction](https://wiki.resonite.com/Component:ArcLayout#Direction)** | How to arrange the elements in order from the initial position. |

Fields
Collapse

## Usage

## Examples

## Related Components

- [ArcSegmentLayout](https://wiki.resonite.com/Component:ArcSegmentLayout "Component:ArcSegmentLayout")
- [OutlinedArc](https://wiki.resonite.com/Component:OutlinedArc "Component:OutlinedArc")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ArcLayout&oldid=97378](https://wiki.resonite.com/index.php?title=Component:ArcLayout&oldid=97378)"

Contents