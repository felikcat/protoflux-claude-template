# Component:HorizontalLayout

> Source: https://wiki.resonite.com/Component:HorizontalLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:HorizontalLayout&diff=88819) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/12/HorizontalLayoutComponent.png/510px-HorizontalLayoutComponent.png)](https://wiki.resonite.com/File:HorizontalLayoutComponent.png) **HorizontalLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Introduction

The **HorizontalLayout** component is used to layout child [UIX](https://wiki.resonite.com/UIX "UIX") element [slots](https://wiki.resonite.com/Slot "Slot") in a row, left to right.

The order of the objects depends on each child's OrderOffset property. Normally these are `0`, but if you change it, the children will be ordered by increasing OrderOffset, with children of equal OrderOffset being ordered by the time they were added to that parent slot.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want to layout the [UIX](https://wiki.resonite.com/UIX "UIX") elements vertically, use the [VerticalLayout](https://wiki.resonite.com/Component:VerticalLayout "Component:VerticalLayout") component instead.


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

The HorizontalLayout component places its child layout elements next to each other, side by side. Their widths are determined by their respective minimum, preferred, and flexible widths according to the following model:

1. The minimum widths of all the child layout elements are added together and the spacing between them is added as well. The result is the minimum width of the HorizontalLayout.
2. The preferred widths of all the child layout elements are added together and the spacing between them is added as well. The result is the preferred width of the HorizontalLayout.
3. If the HorizontalLayout is at its minimum width or smaller, all the child layout elements will also have their minimum width.
4. The closer the HorizontalLayout is to its preferred width, the closer each child layout element will also get to their preferred width.
5. If the HorizontalLayout is wider than its preferred width, it will distribute the extra available space proportionally to the child layout elements according to their respective flexible widths.

For minimum, preferred, and flexible heights of child slots, use [LayoutElement](https://wiki.resonite.com/LayoutElement_(Component) "LayoutElement (Component)").

## Examples

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial video on the Horizontal Layout:

![](https://i.ytimg.com/vi/1-FF9IolGZw/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.10 - Layouts](https://www.youtube-nocookie.com/embed/1-FF9IolGZw?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HorizontalLayout&oldid=88819](https://wiki.resonite.com/index.php?title=Component:HorizontalLayout&oldid=88819)"

Contents