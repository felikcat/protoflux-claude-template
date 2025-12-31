# Component:FixedRectFitterLayout

> Source: https://wiki.resonite.com/Component:FixedRectFitterLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FixedRectFitterLayout&diff=98895) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f5/FixedRectFitterLayoutComponent.png/510px-FixedRectFitterLayoutComponent.png)](https://wiki.resonite.com/File:FixedRectFitterLayoutComponent.png) **FixedRectFitterLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FixedRectFitterLayout** component attempts to fit child elements into the [Component:RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") of the FixedRectFitterLayout slot.

To use a FixedRectFitterLayout at least one child element will need an `OffsetMax` value that is not `[0.0; 0.0]`.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HorizontalAlign` | **[LayoutHorizontalAlignment](https://wiki.resonite.com/Type:LayoutHorizontalAlignment "Type:LayoutHorizontalAlignment")** | The alignment of the content horizontally. |
| `VerticalAlign` | **[LayoutVerticalAlignment](https://wiki.resonite.com/Type:LayoutVerticalAlignment "Type:LayoutVerticalAlignment")** | The alignment of the content vertically. |
| `Mode` | **[FixedRectFitterLayout.FitMode](https://wiki.resonite.com/Component:FixedRectFitterLayout#FitMode)** | How the child elements should attempt to fit into this [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") |
| `AllowShrink` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should the child elements shrink to fit the space if needed. |
| `AllowGrow` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should the child elements grow to fill the space if needed. |

Fields
Collapse

## Usage

The **FixedRectFitterLayout** component computes the bounds of child elements using their computed `OffsetMax` values and attempts to to fit the child elements into the FixedRectFitterLayout's [Component:RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") according to the mode.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FixedRectFitterLayout&oldid=98895](https://wiki.resonite.com/index.php?title=Component:FixedRectFitterLayout&oldid=98895)"

Contents