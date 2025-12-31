# Component:VerticalLayout

> Source: https://wiki.resonite.com/Component:VerticalLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VerticalLayout&diff=88820) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/50/VerticalLayoutComponent.png/510px-VerticalLayoutComponent.png)](https://wiki.resonite.com/File:VerticalLayoutComponent.png) **VerticalLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VerticalLayout** component is used to layout child [UIX](https://wiki.resonite.com/UIX "UIX") element [slots](https://wiki.resonite.com/Slot "Slot") in a column, top to bottom.

The order of the objects depends on each child's OrderOffset property. Normally these are `0`, but if you change it, the children will be ordered by increasing OrderOffset, with children of equal OrderOffset being ordered by the time they were added to that parent slot.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want to layout the [UIX](https://wiki.resonite.com/UIX "UIX") elements horizontally, use the [HorizontalLayout](https://wiki.resonite.com/Component:HorizontalLayout "Component:HorizontalLayout") component instead.


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PaddingTop` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The padding to add, in pixels, at the top of the entire layout. |
| `PaddingRight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The padding to add, in pixels, at the right of the entire layout. |
| `PaddingBottom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The padding to add, in pixels, at the bottom of the entire layout. |
| `PaddingLeft` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The padding to add, in pixels, at the left of the entire layout. |
| `Spacing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The padding to add, in pixels, between each object. |
| `HorizontalAlign` | **[LayoutHorizontalAlignment](https://wiki.resonite.com/Type:LayoutHorizontalAlignment "Type:LayoutHorizontalAlignment")** | The horizontal alignment to use for the child objects in the layout. |
| `VerticalAlign` | **[LayoutVerticalAlignment](https://wiki.resonite.com/Type:LayoutVerticalAlignment "Type:LayoutVerticalAlignment")** | The vertical alignment to use for the child objects in the layout. |
| `ForceExpandWidth` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the children to expand to fill the available horizontal space. |
| `ForceExpandHeight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force the children to expand to fill the available vertical space. |

Fields
Collapse

## Usage

The VerticalLayout component places its child layout elements on top of each other. Their heights are determined by their respective minimum, preferred, and flexible heights according to the following model:

1. The minimum heights of all the child layout elements are added together and the spacing between them plus the top and bottom padding is added as well. The result is the minimum height of the VerticalLayout.
2. The preferred heights of all the child layout elements are added together and the spacing between them plus the top and bottom padding is added as well. The result is the preferred height of the VerticalLayout.
3. If the VerticalLayout is at its minimum height or smaller, all the child layout elements will also have their minimum height.
4. The closer the VerticalLayout is to its preferred height, the closer each child layout element will also get to their preferred height.
5. If the VerticalLayout is taller than its preferred height, it will distribute the extra available space proportionally to the child layout elements according to their respective flexible heights.

For minimum, preferred, and flexible heights of child slots, use [LayoutElement](https://wiki.resonite.com/LayoutElement_(Component) "LayoutElement (Component)").

### Padding and spacing

[![](https://wiki.resonite.com/images/d/dc/Verticallayout_padding.png)](https://wiki.resonite.com/File:Verticallayout_padding.png)

## Examples

This example shows a VerticalLayout with two children. Each child is just an [Image](https://wiki.resonite.com/Image_(Component) "Image (Component)"), with the first child being red and the second being green. Note that since Images have no minimum or preferred size, the VerticalLayout's ForceExpandWidth and ForceExpandHeight properties must be set, otherwise the children will simply have a width or height of zero. The VerticalLayout is as big as its parent allows.

VerticalLayout in the inspector:

[![](https://wiki.resonite.com/images/thumb/2/2e/Vertical_Layout_Example_1_Layout.jpeg/800px-Vertical_Layout_Example_1_Layout.jpeg)](https://wiki.resonite.com/File:Vertical_Layout_Example_1_Layout.jpeg)

The first child in the inspector:

[![](https://wiki.resonite.com/images/thumb/5/57/Vertical_Layout_Example_1_Child.jpeg/800px-Vertical_Layout_Example_1_Child.jpeg)](https://wiki.resonite.com/File:Vertical_Layout_Example_1_Child.jpeg)

The result:

[![](https://wiki.resonite.com/images/thumb/4/4b/Vertical_Layout_Example_1_Result.jpeg/800px-Vertical_Layout_Example_1_Result.jpeg)](https://wiki.resonite.com/File:Vertical_Layout_Example_1_Result.jpeg)

If we add LayoutElements to each child, we can affect the sizes. Here, we add a LayoutElement to the first child, setting its FlexibleHeight to 2, and also to the second child, setting its FlexibleHeight to 1:

[![](https://wiki.resonite.com/images/thumb/4/45/Vertical_Layout_Example_1_Child_with_Layout_Element.jpeg/800px-Vertical_Layout_Example_1_Child_with_Layout_Element.jpeg)](https://wiki.resonite.com/File:Vertical_Layout_Example_1_Child_with_Layout_Element.jpeg)

The result shows that the child heights are proportional, 2 to 1:

[![](https://wiki.resonite.com/images/thumb/1/19/Vertical_Layout_Example_1_Result_with_Layout_Element.jpeg/800px-Vertical_Layout_Example_1_Result_with_Layout_Element.jpeg)](https://wiki.resonite.com/File:Vertical_Layout_Example_1_Result_with_Layout_Element.jpeg)

By specifying a preferred width for each child and turning off ForceExpandWidth on the VerticalLayout, we can have each child stick to its preferred width. Here, we set the first child's preferred width to 100 and the second child's preferred width to 50:

[![](https://wiki.resonite.com/images/thumb/2/29/Vertical_Layout_Example_1_Result_with_Layout_Element_and_Preferred_Width.jpeg/800px-Vertical_Layout_Example_1_Result_with_Layout_Element_and_Preferred_Width.jpeg)](https://wiki.resonite.com/File:Vertical_Layout_Example_1_Result_with_Layout_Element_and_Preferred_Width.jpeg)

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial video on the Vertical Layout:

![](https://i.ytimg.com/vi/1-FF9IolGZw/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.10 - Layouts](https://www.youtube-nocookie.com/embed/1-FF9IolGZw?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VerticalLayout&oldid=88820](https://wiki.resonite.com/index.php?title=Component:VerticalLayout&oldid=88820)"

Contents