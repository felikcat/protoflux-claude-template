# Component:PBS SliceSpecular

> Source: https://wiki.resonite.com/Component:PBS_SliceSpecular

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_SliceSpecular&diff=106116) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3f/PBS_SliceSpecularComponent.png/510px-PBS_SliceSpecularComponent.png)](https://wiki.resonite.com/File:PBS_SliceSpecularComponent.png) **PBS Slice Specular** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A PBS Slice (Metallic & Specular) shader:

- Supports up to 8 plane slicers, cutting a mesh
- Supports slice fade effect along the edge (albedo & emissive)
- Is dual-sided, rendering interior (mesh will look as a shell though)
- Adds a GenericSlicer component, which allows to set the slicing plane visually. To create/edit the material, click "Create Slicer" in the inspector.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `AlbedoColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the albedo (base color) with. Basically a tint. Default white. |
| `EdgeColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the material edge where it is being sliced. |
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the emission (glowly color) with. Basically a tint. Default white. |
| `EdgeEmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The emission color of the edge of the material where it is being sliced. |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `DetailTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different detail texture maps. |
| `DetailTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different detail texture maps. |
| `DetailAlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A multiplied layer of albedo on top of the default `AlbedoTexture`. |
| `DetailNormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A layered normal map on top of the default `NormalMap`. |
| `DetailNormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the detail normal map. |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `HideSlicers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to hide the visuals of the planes for the different slicers. |
| `Slicers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Slicer](https://wiki.resonite.com/Type:Slicer "Type:Slicer")** | A list of slicers (up to 8) that slice this material and create edges. These have a normal and a position in global or local space. |
| `LocalSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to calculate `Distance` and `Point` in local space. |
| `EdgeTransitionStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The place at which the material color at the slicing edge should start transition from 100% slice properties to 0% slice properties to normal material. |
| `EdgeTransitionEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The place at which the material color at the slicing edge should end transitioning from 100% slice properties to 0% slice properties to normal material. |
| `AlphaHandling` | **[AlphaHandling](https://wiki.resonite.com/Type:AlphaHandling "Type:AlphaHandling")** | How to handle alpha values in pixels on the `AlbedoTexture`. |
| `_useAlphaClip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to respect the value for `AlphaClip`. |
| `AlphaClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Any alpha value below this amount is not rendered for any given pixel when cutout is enabled. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_SliceSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_SliceSpecular#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `SpecularColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Specular Tint. Behaves like PBS Specular Tinting |
| `SpecularMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Specular Maps](https://wiki.resonite.com/Component:PBS_Specular#Specular_Maps "Component:PBS Specular") |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_transparent` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Shader, Internal. |

Fields
Collapse

## Usage

## Examples

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_SliceSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_SliceSpecular#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_SliceSpecular&oldid=106116](https://wiki.resonite.com/index.php?title=Component:PBS_SliceSpecular&oldid=106116)"

Contents