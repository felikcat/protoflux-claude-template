# Component:PBS ColorMaskSpecular

> Source: https://wiki.resonite.com/Component:PBS_ColorMaskSpecular

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/PBS_ColorMaskSpecularComponent.png/510px-PBS_ColorMaskSpecularComponent.png)](https://wiki.resonite.com/File:PBS_ColorMaskSpecularComponent.png) **PBS\_ColorMaskSpecular** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PBS\_ColorMaskSpecular** material is a specular material that allows for four distinct colors to be used separately or mixed in on different areas of the surface based on an image map.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `ColorMaskScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scaling of the color mask texture. |
| `ColorMaskOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the color mask texture. |
| `ColorMask` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | What colors behind the material should make it through the filter. |
| `AlbedoColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of `Texture0`. |
| `AlbedoColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of `Texture1`. |
| `AlbedoColor2` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where B is on `ColorMask` |
| `AlbedoColor3` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where A is on `ColorMask` |
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive texture tint for texture 0. |
| `EmissiveColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive texture tint for texture 1. |
| `EmissiveColor2` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where B is on `AlbedoTexture` |
| `EmissiveColor3` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where A is on `AlbedoTexture` |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `Transparent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this should render transparent |
| `ForceZWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enforce writing to the Z-buffer. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_ColorMaskSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_ColorMaskSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `SpecularColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Specular Tint. Behaves like PBS Specular Tinting |
| `SpecularMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Specular Maps](https://wiki.resonite.com/Component:PBS_Specular#Specular_Maps "Component:PBS Specular") |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_transparent` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Shader, Internal. |
| `_zwrite` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Shader, internal. |

Fields
Collapse

## Usage

The `ColorMask` texture is a [color mask](https://wiki.resonite.com/Color_mask "Color mask") that gets mapped to the four albedo/emissive channels to change individual tints for certain parts of the material. Other fields work as described on the [PBS\_Specular](https://wiki.resonite.com/Component:PBS_Specular "Component:PBS Specular") material.

## Examples

## See Also

- [Color masks](https://wiki.resonite.com/Color_masks "Color masks")
- [Component:PBS\_ColorMaskMetallic](https://wiki.resonite.com/Component:PBS_ColorMaskMetallic "Component:PBS ColorMaskMetallic")

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_ColorMaskSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_ColorMaskSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_ColorMaskSpecular&oldid=105841](https://wiki.resonite.com/index.php?title=Component:PBS_ColorMaskSpecular&oldid=105841)"

Contents