# Component:RectTransform

> Source: https://wiki.resonite.com/Component:RectTransform

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RectTransform&diff=96581) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/de/RectTransformComponent.png/510px-RectTransformComponent.png)](https://wiki.resonite.com/File:RectTransformComponent.png) **RectTransform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RectTransform** component defines what space a slot with [UIX](https://wiki.resonite.com/UIX "UIX") components on it will use, based on the total amount of space that has been provided. This is mostly used to encapsulate elements with inside it, then provides options to anchor, offset, and pivot the placement of the RectTransform container.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

When smoothly changing this component's values it will not act with the intended effect. Use [Component:RectTransformLerp](https://wiki.resonite.com/Component:RectTransformLerp "Component:RectTransformLerp") instead.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AnchorMin` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The normalized position (0 to 1) in the parent object that the lower left corner is anchored to. |
| `AnchorMax` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The normalized position (0 to 1) in the parent object that the upper right corner is anchored to. |
| `OffsetMin` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the lower left corner of the rectangle relative to the lower left anchor, in pixels. |
| `OffsetMax` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the upper right corner of the rectangle relative to the upper right anchor, in pixels. |
| `Pivot` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The normalized position in this rectangle that it rotates around. |

Fields
Collapse

## Usage

This can be used for placements inside your canvas or other upper elements, for your images or other lower elements for this container component.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

When attempting to duplicate a RectTransform, the new RectTransform will remove itself from the [slot](https://wiki.resonite.com/Slot "Slot").


## Examples

Here is a video from [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on RectTransforms:

![](https://i.ytimg.com/vi/cLtD7uWrduI/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.1 Canvases and Rectangles](https://www.youtube-nocookie.com/embed/cLtD7uWrduI?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

The [RectTransformComputedProperties](https://wiki.resonite.com/Component:RectTransformComputedProperties "Component:RectTransformComputedProperties") component is useful when using this component as a reference, returning you the size of the actual rect transform for your calculations.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RectTransform&oldid=96581](https://wiki.resonite.com/index.php?title=Component:RectTransform&oldid=96581)"

Contents