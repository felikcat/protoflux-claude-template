# Component:LayoutElement

> Source: https://wiki.resonite.com/Component:LayoutElement

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LayoutElement&diff=88824) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d7/LayoutElementComponent.png/510px-LayoutElementComponent.png)](https://wiki.resonite.com/File:LayoutElementComponent.png) **LayoutElement** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

**LayoutElement** is a component used within [UIX](https://wiki.resonite.com/UIX "UIX"), instructing components in [slots](https://wiki.resonite.com/Slot "Slot") above it in its hierarchy about how large it would like to be in a variety of dimensions and configurations within the UIX Layout flow. It is often used in combination with various other Layout components such as [HorizontalLayout](https://wiki.resonite.com/HorizontalLayout_(Component) "HorizontalLayout (Component)") or [VerticalLayout](https://wiki.resonite.com/VerticalLayout_(Component) "VerticalLayout (Component)"). By configuring its various properties, you can achieve a wide variety of effects and layouts.

Many of these values may have unclear meaning, even with the table below. Please see the behavior section for more information.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum width for this LayoutElement. |
| `PreferredWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The preferred width for this LayoutElement. |
| `FlexibleWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If there is any space left over after layouting, the width is used as a weight to decide what width should given to this LayoutElement. |
| `MinHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum height for this LayoutElement. |
| `PreferredHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The preferred height for this LayoutElement. |
| `FlexibleHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If there is any space left over after layouting, the height is used as a weight to decide what height should be given to this LayoutElement. |
| `Area` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Currently unused. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority for this LayoutElement. |
| `UseZeroMetrics` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If checked, it allows "0" to be used in the other properties within this component. |

Fields
Collapse

## Usage

LayoutElement is used to inform UIX Layout Components in the layout containers and slots above it within the hierarchy about what size it should be. This information is then used within the UIX Layout process with any other UIX Elements to determine an overall Layout.

For Width and Height there are 3 Properties which are used as a sort of negotiation with the UIX layout to determine the final size of an element. Other processes are involved but when it comes to just the layout element, the negotiation uses the following method:

1. Ensure that the element is at least MinWidth/MinHeight in terms of units. If a layout element does not fit inside a parent container/RectTransform it will cause Overflow if these Minimums are too large.
2. If there's enough space, give this element its PreferredWidth/PreferredHeight space in units. If there is not enough space for the "Preferred" value it will use a number that is between the "Min" value and the "Preferred" value.
3. After both 1 and 2, if there is space available and the "Flexible" parameter is set it will give this element a weighted value of space by comparing the Flexible values of all other elements in the layout.

If a parameter should not be used, its value should be set to \`-1\`. You can also manually specify that it should be 0 by checking the "UseZeroMetrics" checkbox.

The priority parameter determines this layout's priority when compared with other elements within the same hierarchy. The highest priority wins. You usually do not need to touch this.

## Examples

### Vertical Layout & FlexibleHeight

Pictured below is a VerticalLayout, with 3 LayoutElements beneath it. The slot hierarchy is as follows:

- VerticalLayout Slot
  - Layout Element Slot 1
  - Layout Element Slot 2
  - Layout Element Slot 3

Each of the Layout Elements has its FlexibleHeight property set to 1, with all other properties set to their default values:

[![](https://wiki.resonite.com/images/thumb/3/37/VerticalLayout.png/250px-VerticalLayout.png)](https://wiki.resonite.com/File:VerticalLayout.png)

In this second picture, the middle element has its FlexibleHeight Property set to 2:

[![](https://wiki.resonite.com/images/thumb/c/c6/VerticalLayoutBigMiddle.png/250px-VerticalLayoutBigMiddle.png)](https://wiki.resonite.com/File:VerticalLayoutBigMiddle.png)

In this case, the VerticalLayout has awarded double the available height space to Layout Element Slot 2.

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial video about Layout Element:

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LayoutElement&oldid=88824](https://wiki.resonite.com/index.php?title=Component:LayoutElement&oldid=88824)"

Contents