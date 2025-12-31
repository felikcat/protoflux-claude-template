# Component:GridLayout

> Source: https://wiki.resonite.com/Component:GridLayout

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GridLayout&diff=88818) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bd/GridLayoutComponent.png/510px-GridLayoutComponent.png)](https://wiki.resonite.com/File:GridLayoutComponent.png) **GridLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GridLayout** component aligns the [UIX](https://wiki.resonite.com/UIX "UIX") elements from left to right, top to bottom. This component also comes with controllable parameters that a [user](https://wiki.resonite.com/User "User") can use to adjust the way the grid layout is represented on the [Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") or element [slot](https://wiki.resonite.com/Slot "Slot").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PaddingTop` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Makes padding on the top of this grid, separating it from the top. |
| `PaddingRight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Makes padding on the right of this grid, separating it from the right. |
| `PaddingBottom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Makes padding on the bottom of this grid, separating it from the bottom. |
| `PaddingLeft` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Makes padding on the left of this grid, separating it from the left. |
| `CellSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of each content cell. |
| `Spacing` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | Makes padding between the content cells of this grid, separating it evenly. |
| `HorizontalAlign` | **[LayoutHorizontalAlignment](https://wiki.resonite.com/Type:LayoutHorizontalAlignment "Type:LayoutHorizontalAlignment")** | how this grid should be aligned horizontally. |
| `VerticalAlign` | **[LayoutVerticalAlignment](https://wiki.resonite.com/Type:LayoutVerticalAlignment "Type:LayoutVerticalAlignment")** | how this grid should be aligned vertically. |
| `ExpandWidthToFit` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Extends this grid to fit the entire [UIX](https://wiki.resonite.com/UIX "UIX") element that it is on. |
| `PreserveAspectOnExpand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Preserves the aspect ratio when expanded to fit. |
| `AlignLastRowIndividually` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Alighns the last row for this grid seprately. |

Fields
Collapse

## Usage

This is used to make a nice grid layout of a user's content. The user has a lot of control when it comes to making this kind of layout, especially when it comes to the amount of content cells, expanding and scaling those cells, and alignments.

## Examples

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial video on the Grid Layout:

![](https://i.ytimg.com/vi/1-FF9IolGZw/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.10 - Layouts](https://www.youtube-nocookie.com/embed/1-FF9IolGZw?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GridLayout&oldid=88818](https://wiki.resonite.com/index.php?title=Component:GridLayout&oldid=88818)"

Contents