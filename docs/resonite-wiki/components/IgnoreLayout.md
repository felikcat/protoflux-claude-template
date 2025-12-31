# Component:IgnoreLayout

> Source: https://wiki.resonite.com/Component:IgnoreLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:IgnoreLayout&diff=91540) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d7/IgnoreLayoutComponent.png/510px-IgnoreLayoutComponent.png)](https://wiki.resonite.com/File:IgnoreLayoutComponent.png) **IgnoreLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **IgnoreLayout** component makes a [UIX](https://wiki.resonite.com/UIX "UIX") element ignore the parent [slot](https://wiki.resonite.com/Slot "Slot")'s layout component, and then draws over other elements (within that same hierarchy level of slots) inside of the parent's [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Attach to a slot which the elements within should ignore the layout of the parent slot.

## Examples

Useful if you need to make a pop-up or to draw over something in [UIX](https://wiki.resonite.com/UIX "UIX").

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:IgnoreLayout&oldid=91540](https://wiki.resonite.com/index.php?title=Component:IgnoreLayout&oldid=91540)"

Contents