# Component:ScrollRect

> Source: https://wiki.resonite.com/Component:ScrollRect

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScrollRect&diff=98052) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/48/ScrollRectComponent.png/510px-ScrollRectComponent.png)](https://wiki.resonite.com/File:ScrollRectComponent.png) **ScrollRect** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScrollRect** component is for making the contents of this [Slot](https://wiki.resonite.com/Slot "Slot") (such as child objects with [RectTransforms](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")) scrollable.

The scrollRect will not do any clipping on its own. If it is a child of an object with a [Mask](https://wiki.resonite.com/Component:Mask "Component:Mask") component, it effectively becomes a window into the scrolled content.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

It is recommended to use a [ContentSizeFitter](https://wiki.resonite.com/Component:ContentSizeFitter "Component:ContentSizeFitter") component and setting the `VerticalFit` to `MinSize` when combined with a scrollrect to help fit it within a [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform").


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `NormalizedPosition` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scroll position between (0,0) and (1,1) with (0,0) being the lower left corner. |
| `HorizontalAlign` | **[LayoutHorizontalAlignment](https://wiki.resonite.com/Type:LayoutHorizontalAlignment "Type:LayoutHorizontalAlignment")** | Aligns the scrollrect's contents horizontal. |
| `VerticalAlign` | **[LayoutVerticalAlignment](https://wiki.resonite.com/Type:LayoutVerticalAlignment "Type:LayoutVerticalAlignment")** | Aligns the scrollrect's contents vertically. |
| `ViewportOverride` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | Overrides the viewport of this scrollrect. |
| `__legacyContent` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | Internal - Used for the content of the scrollrect. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `MoveToTop:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Moves the scroll view to the top. |
| `MoveToBottom:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Mobes the scroll view to the bottom. |
| `MoveToLeft:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Moves the scroll view to the left. |
| `MoveToRight:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Moves the scroll view to the right. |

Triggers
Collapse

## Usage

This is useful when you have a lot of text or other [UIX](https://wiki.resonite.com/UIX "UIX") elements that you want to be scrollable, much like how a webpage has a lot of content that can't fit in just one screen.

## Examples

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial video on the scrollrect component:

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [UIX](https://wiki.resonite.com/UIX "UIX")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScrollRect&oldid=98052](https://wiki.resonite.com/index.php?title=Component:ScrollRect&oldid=98052)"

Contents