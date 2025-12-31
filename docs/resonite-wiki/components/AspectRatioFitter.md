# Component:AspectRatioFitter

> Source: https://wiki.resonite.com/Component:AspectRatioFitter

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AspectRatioFitter&diff=88805) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ab/AspectRatioFitterComponent.png/510px-AspectRatioFitterComponent.png)](https://wiki.resonite.com/File:AspectRatioFitterComponent.png) **AspectRatioFitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AspectRatioFitter** component makes the contents (child [slots](https://wiki.resonite.com/Slot "Slot")) of the [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") stay the same dimensions (or the same ratio), even when the canvas or [UIX](https://wiki.resonite.com/UIX "UIX") element this component is in changes size.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AspectRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The aspect ratio of this UIX element. `1` is a perfect square, less than `1` is a vertical ratio, greater than `1` is a horizontal ratio. |

Fields
Collapse

## Usage

Great for keeping things more uniform by a ratio.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AspectRatioFitter&oldid=88805](https://wiki.resonite.com/index.php?title=Component:AspectRatioFitter&oldid=88805)"

Contents