# Component:DualColorImage

> Source: https://wiki.resonite.com/Component:DualColorImage

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DualColorImage&diff=91585) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a4/DualColorImageComponent.png/510px-DualColorImageComponent.png)](https://wiki.resonite.com/File:DualColorImageComponent.png) **DualColorImage** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DualColorImage** component takes in a [SpriteProvider](https://wiki.resonite.com/Component:SpriteProvider "Component:SpriteProvider") or [Material](https://wiki.resonite.com/Material "Material") and controls the tint and secondary tint of a [UIX](https://wiki.resonite.com/UIX "UIX") image. There are optional placement parameters allowing the [user](https://wiki.resonite.com/User "User") to adjust the offset of this image using `FillRect`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

You must have an image that it can register and use, else it will just use the secondary tint color only and fill in the entire area.


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Sprite` | **[Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite")** | The sprite to use as the image. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The Material to use as the image. |
| `PreserveAspect` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Preserves the aspect ratio of this image provided. |
| `NineSliceSizing` | **[NineSliceSizing](https://wiki.resonite.com/Type:NineSliceSizing "Type:NineSliceSizing")** | Tells how the image gets 9-sliced on this UIX. |
| `FlipHorizontally` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the image horizontally. |
| `FlipVertically` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the image vertically. |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this image as the interaction target for this UIX. |
| `FillRect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The filling rect for this image. |
| `__legacyZWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The legacy Z writing for this image. |
| `Tint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The primary tint color for this image. |
| `SecondaryTint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The secondary tint color for this image. |

Fields
Collapse

## Usage

## Examples

This can be used as a way to make an image and give it a tint color.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DualColorImage&oldid=91585](https://wiki.resonite.com/index.php?title=Component:DualColorImage&oldid=91585)"

Contents