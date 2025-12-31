# Component:ContentSizeFitter

> Source: https://wiki.resonite.com/Component:ContentSizeFitter

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ContentSizeFitter&diff=91565) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/60/ContentSizeFitterComponent.png/510px-ContentSizeFitterComponent.png)](https://wiki.resonite.com/File:ContentSizeFitterComponent.png) **ContentSizeFitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ContentSizeFitter** resizes the slots's [RectTransform](https://wiki.resonite.com/RectTransform_(Component) "RectTransform (Component)") to fit the minimum or preferred size of its other _layout_ components in width or height. In effect, it "shrink-wraps" its contents.

Note that this does not include its children slots, and only works on slots that have a layout component. For working with children, the parent with the ContentSizeFitter needs to also have a [HorizontalLayout](https://wiki.resonite.com/HorizontalLayout_(Component) "HorizontalLayout (Component)"), [VerticalLayout](https://wiki.resonite.com/VerticalLayout_(Component) "VerticalLayout (Component)"), or [GridLayout](https://wiki.resonite.com/GridLayout_(Component) "GridLayout (Component)") component. [LayoutElement](https://wiki.resonite.com/LayoutElement_(Component) "LayoutElement (Component)") is also a layout component, as is [Text](https://wiki.resonite.com/Text_(Component) "Text (Component)") and [Image](https://wiki.resonite.com/Image_(Component) "Image (Component)").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HorizontalFit` | **[SizeFit](https://wiki.resonite.com/Type:SizeFit "Type:SizeFit")** | The fit mode to use to determine the width. |
| `VerticalFit` | **[SizeFit](https://wiki.resonite.com/Type:SizeFit "Type:SizeFit")** | The fit mode to use to determine the height. |

Fields
Collapse

Fit modes are:

- Disabled: Don't perform any resizing.
- MinSize: Resize to the minimum size of the content.
- PreferredSize: Resize to the preferred size of the content.

## Usage

This is used for a polished look of keeping your contents in the bounds of a [UIX](https://wiki.resonite.com/UIX "UIX") element.

## Behavior

The ContentSizeFitter functions as a layout controller that controls the size of its own layout component. The size is determined by the minimum or preferred sizes provided by layout components its own slot. Such layout components can be Image or Text components, VerticalLayout, HorizontalLayout, or a LayoutElement component.

## Examples

In this example, we'll "shrink-wrap" the example from the [VerticalLayout](https://wiki.resonite.com/VerticalLayout_(Component) "VerticalLayout (Component)") page. We do this by adding a ContentSizeFitter to the slot with the VerticalLayout, and setting its HorizontalFit mode to PreferredSize. Since the preferred width of the vertical layout is simply the maximum of its children's preferred widths plus the left and right spacing, the vertical layout shrinks horizontally to equal that preference:

[![](https://wiki.resonite.com/images/thumb/b/b4/Content_Size_Fitter_Example_1_Horizontal_Result.jpeg/800px-Content_Size_Fitter_Example_1_Horizontal_Result.jpeg)](https://wiki.resonite.com/File:Content_Size_Fitter_Example_1_Horizontal_Result.jpeg)

If, however, we now also attempt to shrink-wrap vertically by setting the ContentSizeFitter's VerticalFit to PreferredSize, we end up with no colored boxes. This is because the children have their preferred heights set to -1, and that means the heights will simply be set to zero.

[![](https://wiki.resonite.com/images/thumb/5/56/Content_Size_Fitter_Example_1_Vertical_Result_with_no_preferred_height.jpeg/800px-Content_Size_Fitter_Example_1_Vertical_Result_with_no_preferred_height.jpeg)](https://wiki.resonite.com/File:Content_Size_Fitter_Example_1_Vertical_Result_with_no_preferred_height.jpeg)

We can fix this by assigning each child's LayoutElement a preferred height. For example:

[![](https://wiki.resonite.com/images/thumb/0/03/Content_Size_Fitter_Example_1_Vertical_Result_with_preferred_height.jpeg/800px-Content_Size_Fitter_Example_1_Vertical_Result_with_preferred_height.jpeg)](https://wiki.resonite.com/File:Content_Size_Fitter_Example_1_Vertical_Result_with_preferred_height.jpeg)

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContentSizeFitter&oldid=91565](https://wiki.resonite.com/index.php?title=Component:ContentSizeFitter&oldid=91565)"

Contents