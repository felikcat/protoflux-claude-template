# Component:ArcSegmentLayout

> Source: https://wiki.resonite.com/Component:ArcSegmentLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ArcSegmentLayout&diff=88802) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7d/ArcSegmentLayoutComponent.png/510px-ArcSegmentLayoutComponent.png)](https://wiki.resonite.com/File:ArcSegmentLayoutComponent.png) **ArcSegmentLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ArcSegmentLayout** component is used with [ArcLayout](https://wiki.resonite.com/Component:ArcLayout "Component:ArcLayout"), and separates the arc layout into equal segments defined in that component. When using this component, it will be very resistant to change as it is listening on the [ArcLayout](https://wiki.resonite.com/Component:ArcLayout "Component:ArcLayout") for the art amount, size, and ratios.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Nested` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The rect transform to hold the segments of the arc layout. |
| `NestedSizeRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size ratio for this arc segment. |
| `Label` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The label text for the arc segment. |
| `LabelSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The label text size for the arc segment. |
| `LabelDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The label text distance from the arc segment. |

Fields
Collapse

## Usage

This is used for the individual arc segment selection of the [context menu](https://wiki.resonite.com/Context_menu "Context menu").

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ArcSegmentLayout&oldid=88802](https://wiki.resonite.com/index.php?title=Component:ArcSegmentLayout&oldid=88802)"

Contents