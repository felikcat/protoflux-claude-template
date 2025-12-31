# Component:RawGraphic

> Source: https://wiki.resonite.com/Component:RawGraphic

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RawGraphic&diff=88810) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/RawGraphicComponent.png/510px-RawGraphicComponent.png)](https://wiki.resonite.com/File:RawGraphicComponent.png) **RawGraphic** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RawGraphic** component takes in a [Material](https://wiki.resonite.com/Material "Material") or a [Material Property Block](https://wiki.resonite.com/Material_Property_Block "Material Property Block") component, then shows the raw graphic image onto the [UIX](https://wiki.resonite.com/UIX "UIX").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to take the raw graphic from. |
| `PropertyBlock` | **[MaterialPropertyBlock](https://wiki.resonite.com/index.php?title=Type:MaterialPropertyBlock&action=edit&redlink=1 "Type:MaterialPropertyBlock (page does not exist)")** | The image within a literal image block. |
| `FillRect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The filling rect for this image. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Changes the color of the image. |
| `UVRect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | Shifts the UV of the raw image. |
| `Orientation` | **[RectOrientation](https://wiki.resonite.com/index.php?title=Type:RectOrientation&action=edit&redlink=1 "Type:RectOrientation (page does not exist)")** | Rotates the raw image and respects aspect ratio. |
| `Normal` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The normal for this raw graphic. |
| `Tangent` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4") >** | The tangent for this raw graphic. |
| `HideWithNoMaterial` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If there is no material, hid this raw image. |
| `PreserveUVAspectRatio` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If this raw graphic should preserve its aspect ratio. |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this image as the interaction target for this UIX. |

Fields
Collapse

## Usage

Use this component when the [Image](https://wiki.resonite.com/Component:Image "Component:Image") component does not have what your looking for in your [UIX](https://wiki.resonite.com/UIX "UIX") design.

## Examples

## Related Components

- [MainTexturePropertyBlock](https://wiki.resonite.com/Component:MainTexturePropertyBlock "Component:MainTexturePropertyBlock")
- [Projection360PropertyBlock](https://wiki.resonite.com/Component:Projection360PropertyBlock "Component:Projection360PropertyBlock")
- [MainAndMaskTexturePropertyBlock](https://wiki.resonite.com/Component:MainAndMaskTexturePropertyBlock "Component:MainAndMaskTexturePropertyBlock")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RawGraphic&oldid=88810](https://wiki.resonite.com/index.php?title=Component:RawGraphic&oldid=88810)"

Contents