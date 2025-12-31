# Component:Mask

> Source: https://wiki.resonite.com/Component:Mask

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Mask&diff=96636) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/66/MaskComponent.png/510px-MaskComponent.png)](https://wiki.resonite.com/File:MaskComponent.png) **Mask** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Mask** component restricts the rendering of anything beneath it. It requires an [Image](https://wiki.resonite.com/Component:Image "Component:Image") component, [text](https://wiki.resonite.com/Component:Text "Component:Text"), [arc](https://wiki.resonite.com/Component:OutlinedArc "Component:OutlinedArc"), [rectmesh](https://wiki.resonite.com/Component:RectMesh "Component:RectMesh"), or anything that displays a graphic on the same [slot](https://wiki.resonite.com/Slot "Slot"). Only opaque areas of the graphic on the same slot will render the [UIX](https://wiki.resonite.com/UIX "UIX") below. This is also utilized in [ScrollRect](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect") since it can mask anything outside of the scrolling viewport when using the component.

There is a [UIX Tutorial](https://wiki.resonite.com/UIX_Tutorial "UIX Tutorial") that use masking and [ScrollRects](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect") to help you understand how masks work.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

A few notes about this component:

- This can have issues with UIX's behind, since there are some rendering bugs with Unity.
- If a **Mask** component and a layout component ( [HorizontalLayout](https://wiki.resonite.com/Component:HorizontalLayout "Component:HorizontalLayout"), [VerticalLayout](https://wiki.resonite.com/Component:VerticalLayout "Component:VerticalLayout"), or [GridLayout](https://wiki.resonite.com/Component:GridLayout "Component:GridLayout")) are on the same slot, it will mess up the UIX (especially when trying to make [ScrollRects](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect") work).

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ShowMaskGraphic` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Shows the graphic being used to do the masking for debug purposes. |

Fields
Collapse

## Usage

This can be used for fancy cutout effects.

## Examples

The [ScrollRect](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect") section which is part of the [UIX](https://wiki.resonite.com/UIX "UIX") Canvas object created by the [create new menu](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard").

Here is [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on masking:

![](https://i.ytimg.com/vi/WPL776reVFw/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.5 - Masking Images & Nine Slicing](https://www.youtube-nocookie.com/embed/WPL776reVFw?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Mask&oldid=96636](https://wiki.resonite.com/index.php?title=Component:Mask&oldid=96636)"

Contents