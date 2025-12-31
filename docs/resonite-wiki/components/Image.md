# Component:Image

> Source: https://wiki.resonite.com/Component:Image

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Image&diff=91468) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d5/ImageComponent.png/510px-ImageComponent.png)](https://wiki.resonite.com/File:ImageComponent.png) **Image** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Image** component takes in a [SpriteProvider](https://wiki.resonite.com/Component:SpriteProvider "Component:SpriteProvider") or [Material](https://wiki.resonite.com/Material "Material") and renders it onto the [UIX](https://wiki.resonite.com/UIX "UIX"). This can be used to display graphics and produce backgrounds.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Sprite` | **[Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite")** | The sprite to render |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to render with. is not required. |
| `PreserveAspect` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Preserves the aspect ratio of this image provided. |
| `NineSliceSizing` | **[NineSliceSizing](https://wiki.resonite.com/Type:NineSliceSizing "Type:NineSliceSizing")** | Tells how the image gets 9-sliced on this UIX. |
| `FlipHorizontally` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the image horizontally. |
| `FlipVertically` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the image vertically. |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this image as the interaction target for this UIX. |
| `FillRect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The filling rect for this image. |
| `__legacyZWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Internal - The legacy Z writing for this image. |
| `Tint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | A color that is multiplied with the material's color. |

Fields
Collapse

## Usage

A user can use this to just display an image with an optional tint color, or have this as a background image for other images to be on top of.

## Examples

Here is [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on images:

![](https://i.ytimg.com/vi/FUUSjTwhvHk/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.4 - Images & Sprites](https://www.youtube-nocookie.com/embed/FUUSjTwhvHk?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Image&oldid=91468](https://wiki.resonite.com/index.php?title=Component:Image&oldid=91468)"

Contents