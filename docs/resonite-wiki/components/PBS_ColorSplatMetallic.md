# Component:PBS ColorSplatMetallic

> Source: https://wiki.resonite.com/Component:PBS_ColorSplatMetallic

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_ColorSplatMetallic&diff=105842) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bf/PBS_ColorSplatMetallicComponent.png/510px-PBS_ColorSplatMetallicComponent.png)](https://wiki.resonite.com/File:PBS_ColorSplatMetallicComponent.png) **PBS Color Splat Metallic** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A PBS Color Splat (Metallic & Specular) shader:

- Supports 4 textures of each and a color map, where each channel represents contribution from each
- Supports height map blending too for sharper, more defined look
- Is useful for terrains

See also: [Color Splat Materials](https://wiki.resonite.com/Color_Splat_Materials "Color Splat Materials")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `MultiValue` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Multiplies the constant value versions of packed texture information with the corrosponding channel of the packed image. |
| `ColorMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The color splat map to specify what textures go where. |
| `ColorMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of the color splat map. |
| `ColorMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the color splat map. |
| `PackedHeightMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [#Packed Textures Channel Mappings](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#Packed_Textures_Channel_Mappings). |
| `HeightTransitionRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | From 0 to this number is the encoding of the height map data. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `AlbedoColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of `Texture0`. |
| `AlbedoColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color tint of `Texture1`. |
| `AlbedoColor2` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where B is on `ColorMask` |
| `AlbedoColor3` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where A is on `ColorMask` |
| `AlbedoTexture0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Texture 0 for albedo. |
| `AlbedoTexture1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Texture 1 for albedo. |
| `AlbedoTexture2` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Albedo map 2. |
| `AlbedoTexture3` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Albedo map 3. |
| `EmissiveColor0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive texture tint for texture 0. |
| `EmissiveColor1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emissive texture tint for texture 1. |
| `EmissiveColor2` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where B is on `AlbedoTexture` |
| `EmissiveColor3` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for spots where A is on `AlbedoTexture` |
| `EmissiveMap0` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture 0 for emissive. |
| `EmissiveMap1` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture 1 for emissive. |
| `EmissiveMap2` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The color map for emissive 2. |
| `EmissiveMap3` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The color map for emissive 3. |
| `PackedEmissionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [#Packed Textures Channel Mappings](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#Packed_Textures_Channel_Mappings). |
| `PackedNormalMap01` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [#Packed Textures Channel Mappings](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#Packed_Textures_Channel_Mappings). |
| `PackedNormalMap23` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [#Packed Textures Channel Mappings](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#Packed_Textures_Channel_Mappings). |
| `NormalScale0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The normal scale for normal 0. |
| `NormalScale1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The normal scale for normal 1. |
| `NormalScale2` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scaling of normal map 2. |
| `NormalScale3` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scaling of normal map 3. |
| `AlphaClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum threshold for alpha which before this value it will be not rendered for that pixel. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `Metallic0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The metallicness for set 0 when a texture is not provided for set 0. |
| `Metallic1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The metallicness for set 1 when a texture is not provided for set 1. |
| `Metallic2` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Metallicness of map 2 in absence of `MetallicMap23`. |
| `Metallic3` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Metallicness of map 3 in absence of `MetallicMap23`. |
| `Smoothness0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smoothness for set 0 when a texture is not provided for set 0. |
| `Smoothness1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smoothness for set 1 when a texture is not provided for set 1. |
| `Smoothness2` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Smoothness of map 2 in absence of `MetallicMap23`. |
| `Smoothness3` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Smoothness of map 3 in absence of `MetallicMap23`. |
| `MetallicMap01` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [#Packed Textures Channel Mappings](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#Packed_Textures_Channel_Mappings). |
| `MetallicMap23` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [#Packed Textures Channel Mappings](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#Packed_Textures_Channel_Mappings). |

Fields
Collapse

## Usage

For comprehensive guides see [Color Splat Materials](https://wiki.resonite.com/Color_Splat_Materials "Color Splat Materials").

## Packed Textures Channel Mappings

**PackedEmissionMap** is greyscale and uses **EmissiveColor0-3** Colors.

**EmissiveMap0-3** can be used for RGB Emissive Maps.

Referencing a **PackedEmissionMap** Overrides **EmissiveMap0-3** Inputs.

**PackedHeightMap:****R:** HeightMap0 - greyscale**G:** HeightMap1 - greyscale**B:** HeightMap2 - greyscale**A:** HeightMap4 - greyscale**PackedEmissionMap:****R:** EmissionMap0 - greyscale**G:** EmissionMap1 - greyscale**B:** EmissionMap2 - greyscale**A:** EmissionMap4 - greyscale**PackedNormalMap01:****R:** NormalMap0 - Red**G:** NormalMap0 - Green**B:** NormalMap1 - Red**A:** NormalMap1 - Green**PackedNormalMap23:****R:** NormalMap2 - Red**G:** NormalMap2 - Green**B:** NormalMap3 - Red**A:** NormalMap3 - Green**MetallicMap01:****R:** MetallicMap0 - Red**G:** MetallicMap0 - Alpha**B:** MetallicMap1 - Red**A:** MetallicMap1 - Alpha**MetallicMap23:****R:** MetallicMap2 - Red**G:** MetallicMap2 - Alpha**B:** MetallicMap3 - Red**A:** MetallicMap3 - Alpha

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Used in terrain mostly.

## See Also

- [Component:PBS\_ColorSplatSpecular](https://wiki.resonite.com/Component:PBS_ColorSplatSpecular "Component:PBS ColorSplatSpecular")
- [Color Splat Materials](https://wiki.resonite.com/Color_Splat_Materials "Color Splat Materials")
- [Component:TextureCharacterControllerModifier](https://wiki.resonite.com/Component:TextureCharacterControllerModifier "Component:TextureCharacterControllerModifier")

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_ColorSplatMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_ColorSplatMetallic&oldid=105842](https://wiki.resonite.com/index.php?title=Component:PBS_ColorSplatMetallic&oldid=105842)"

Contents