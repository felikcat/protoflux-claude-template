# Component:RectTransformComputedProperties

> Source: https://wiki.resonite.com/Component:RectTransformComputedProperties

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/42/RectTransformComputedPropertiesComponent.png/510px-RectTransformComputedPropertiesComponent.png)](https://wiki.resonite.com/File:RectTransformComputedPropertiesComponent.png) **Rect Transform Computed Properties** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RectTransformComputedProperties** component is used to get the real size of a [UIX](https://wiki.resonite.com/UIX "UIX") element that is contained in a [slot](https://wiki.resonite.com/Slot "Slot") that has a [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform"). It takes in the RectTransform reference, and then returns a `LocalComputerRect`, which is the local bounds of the element, and returns the `BoundingRect`, which is the bounding rect itself (which can be larger than the local elements from within). Most of the time, both values would be the same, except for some situations.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Rect` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The rect transform component to reference from |
| `LocalComputeRect` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The local bounds of the element |
| `BoundingRect` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The bounding rect itself |

Fields
Collapse

## Usage

This is used to get the size of the bounds of whatever is inside the [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

The [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") component is needed for this component to work.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RectTransformComputedProperties&oldid=113734](https://wiki.resonite.com/index.php?title=Component:RectTransformComputedProperties&oldid=113734)"

Contents