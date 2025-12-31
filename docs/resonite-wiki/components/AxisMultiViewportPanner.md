# Component:AxisMultiViewportPanner

> Source: https://wiki.resonite.com/Component:AxisMultiViewportPanner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AxisMultiViewportPanner&diff=97404) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a9/AxisMultiViewportPannerComponent.png/510px-AxisMultiViewportPannerComponent.png)](https://wiki.resonite.com/File:AxisMultiViewportPannerComponent.png) **AxisMultiViewportPanner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisMultiViewportPanner** component toggles through [UIX](https://wiki.resonite.com/UIX "UIX") element's active state, min and max of the [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")'s anchor. This allows a [user](https://wiki.resonite.com/User "User") to make "pages" in UIX.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ViewportIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The current focused viewport [UIX](https://wiki.resonite.com/UIX "UIX") element. |
| `AnimationTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The time it takes to pan across to get to the selected viewport index. |
| `Direction` | **[AxisMultiViewportPanner.AlignDirection](https://wiki.resonite.com/Component:AxisMultiViewportPanner#AlignDirection)** | The direction this animates to get to the selected viewport index. |
| `Viewports` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AxisMultiViewportPanner.Viewport](https://wiki.resonite.com/Component:AxisMultiViewportPanner#Viewport)** | The list of [UIX](https://wiki.resonite.com/UIX "UIX") element viewports to pan to. |

Fields
Collapse

## Usage

This is useful if you want to make a slideshow, tab pages for [UIX](https://wiki.resonite.com/UIX "UIX"), or anything that you want to have pan across for multiple pages in your design.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component does not have the capability of jumping or skipping from on page directly to the next while also using the animation time. It will go through each page one at a time to get to the destination. If you want to have the functionality to jump to a page, you will need to do a bit of math currently.


## Examples

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial video about the AxisMultiViewportPanner:

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisMultiViewportPanner&oldid=97404](https://wiki.resonite.com/index.php?title=Component:AxisMultiViewportPanner&oldid=97404)"

Contents