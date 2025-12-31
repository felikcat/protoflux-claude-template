# Component:GradientImage

> Source: https://wiki.resonite.com/Component:GradientImage

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/GradientImageComponent.png/510px-GradientImageComponent.png)](https://wiki.resonite.com/File:GradientImageComponent.png) **Gradient Image** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GradiantImage** component takes in a [SpriteProvider](https://wiki.resonite.com/Component:SpriteProvider "Component:SpriteProvider") or [Material](https://wiki.resonite.com/Material "Material") and controls the image color using the four corners of the image, then gradients them into the image.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Sprite` | **[Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite")** | The sprite to use as the image. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The Material to use as the image. |
| `PreserveAspect` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Preserves the aspect ratio of this image provided. |
| `NineSliceSizing` | **[NineSliceSizing](https://wiki.resonite.com/Type:NineSliceSizing "Type:NineSliceSizing")** | Tells how the image gets 9-sliced on this UIX. |
| `FlipHorizontally` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the image horizontally (but not the color). |
| `FlipVertically` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Flips the image vertically (but not the color). |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this image as the interaction target for this UIX. |
| `FillRect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The filling rect for this image. |
| `__legacyZWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The legacy Z writing for this image. |
| `TintTopLeft` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this top left corner. |
| `TintTopRight` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this top right corner. |
| `TintBottomRight` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this bottom right corner. |
| `TintBottomLeft` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this bottom left corner. |

Fields
Collapse

## Usage

You can make fancy effects and icons using this component, especially if your hue shifting the different color corners.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GradientImage&oldid=88615](https://wiki.resonite.com/index.php?title=Component:GradientImage&oldid=88615)"

Contents