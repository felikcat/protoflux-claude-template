# Component:OutlinedArc

> Source: https://wiki.resonite.com/Component:OutlinedArc

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:OutlinedArc&diff=91542) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/53/OutlinedArcComponent.png/510px-OutlinedArcComponent.png)](https://wiki.resonite.com/File:OutlinedArcComponent.png) **OutlinedArc** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OutlinedArc** component takes in many parameters to create a circular image or design and can be controlled using those parameters. Then this renders onto the [UIX](https://wiki.resonite.com/UIX "UIX").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to arc around the center. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to rotate around the center. |
| `OuterRadiusRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The outer distance for this arc from the center. |
| `InnerRadiusRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The inner distance for this arc from the center. |
| `RoundedCornerRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of how rounded the edges of the arc end points are. |
| `FillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The inner color (filled in color) of this arc. |
| `OutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The outer color (the outline) of this arc. |
| `OutlineThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to thicken for the outline. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | Uses a material for the arc. |

Fields
Collapse

## Usage

A user could make fancy effects like a [loading circular throbber](https://en.wikipedia.org/wiki/Throbber), or menu buttons that arc around.

## Examples

Similar to how the [context menu](https://wiki.resonite.com/Context_menu "Context menu") arcs around.

## Related Components

- [Context menu components](https://wiki.resonite.com/Category:Components:Radiant_UI:Context_Menu "Category:Components:Radiant UI:Context Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OutlinedArc&oldid=91542](https://wiki.resonite.com/index.php?title=Component:OutlinedArc&oldid=91542)"

Contents