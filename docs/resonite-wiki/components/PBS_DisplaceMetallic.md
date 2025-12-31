# Component:PBS DisplaceMetallic

> Source: https://wiki.resonite.com/Component:PBS_DisplaceMetallic

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PBS_DisplaceMetallic&diff=105844) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ad/PBS_DisplaceMetallicComponent.png/510px-PBS_DisplaceMetallicComponent.png)](https://wiki.resonite.com/File:PBS_DisplaceMetallicComponent.png) **PBS Displace Metallic** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PBS\_DisplaceMetallic** component can displace the vertices of a mesh _in the direction of the vertex's normal_ via the VertexDisplaceMap settings and the WorldSpaceVertexOffsetMap.

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
| `AlbedoTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the color of the surface. |
| `EmissiveColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to multiply the texture of the emission (glowly color) with. Basically a tint. Default white. |
| `EmissiveMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to use as the glowing (emission) color of the surface. |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `NormalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the effect of the normal map. |
| `OcclusionMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Used to specify surface parts in eternal shadow due to being close to other mesh parts. |
| `VertexDisplaceMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [VertexDisplaceMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#VertexDisplaceMap). |
| `VertexDisplaceMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [VertexDisplaceMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#VertexDisplaceMap). |
| `VertexDisplaceBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [VertexDisplaceMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#VertexDisplaceMap). |
| `VertexDisplaceMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [VertexDisplaceMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#VertexDisplaceMap). |
| `VertexDisplaceMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [VertexDisplaceMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#VertexDisplaceMap). |
| `UVDisplaceMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | A map to displace the UV coordinates of the mesh for every other texture. |
| `UVDisplaceMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How strong the UV displace effect is. |
| `UVDisplaceBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to add to the uv displacement. |
| `UVDisplaceMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV scale of the displacement map for UVs on the original surface. |
| `UVDisplaceMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The UV offset of the displacement map for UVs on the original surface. |
| `WorldspaceVertexOffsetMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | See [WorldSpaceVertexOffsetMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#WorldSpaceVertexOffsetMap). |
| `WorldspaceOffsetMagnitude` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [WorldSpaceVertexOffsetMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#WorldSpaceVertexOffsetMap). |
| `WorldspaceVertexOffsetMapScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [WorldSpaceVertexOffsetMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#WorldSpaceVertexOffsetMap). |
| `WorldspaceVertexOffsetMapOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [WorldSpaceVertexOffsetMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#WorldSpaceVertexOffsetMap). |
| `WorldspaceOffsetPerVertex` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | See [WorldSpaceVertexOffsetMap](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#WorldSpaceVertexOffsetMap). |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `AlphaHandling` | **[AlphaHandling](https://wiki.resonite.com/Type:AlphaHandling "Type:AlphaHandling")** | How to handle alpha values in pixels on the `AlbedoTexture`. |
| `AlphaClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Any alpha value below this amount is not rendered for any given pixel when cutout is enabled. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `Metallic` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much metallicness the surface should have if `MetallicMap` is not specified. |
| `Smoothness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much smoothness the surface should have if `MetallicMap` is not specified. |
| `MetallicMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Metallic Maps](https://wiki.resonite.com/Component:PBS_Metallic#Metallic_Maps "Component:PBS Metallic") |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_transparent` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Shader, Internal. |

Fields
Collapse

## Usage

The PBS Displace Metallic shader can displace the vertices of a mesh _in the direction of the vertex's normal_ via the VertexDisplaceMap settings and the WorldSpaceVertexOffsetMap.

### VertexDisplaceMap

The texture is an intensity map, so it goes from 0 (black) to 1 (white). Every vertex in the mesh is displaced along its normal _by the same factor_ according to the following formula:

V'n ← Vn \+ Nn x \[ T'(x,y) x M + B \]

where:

- V'n is the displaced position of vertex n.
- Vn is the original position of vertex n.
- Nn is the normal vector for vertex n.
- T(x,y) is the texture map, where x and y are in the range \[-1,1\], and T(x,y) is in the range \[0,1\].
- T'(x,y) is the texture map after it has been scaled by VertexDisplaceMapScale and offset by VertexDisplaceMapOffset.
- M is the VertexDisplacementMagnitude.
- B is the VertexDisplaceBias.
- x and y are 0 (but see WorldSpaceVertexOffsetMap below).

It is important to realize that (x,y) is simply the position in the texture that the swing of each vertex is based off of. It has nothing to do with the positions of the vertices.

Thus:

- T, along with VertexDisplaceMapScale and VertexDisplaceMapOffset, affects the "swing" of the vertex about its original position, in the range \[0,1\], along the direction of the vertex's normal.
- N is the direction and base amplitude of the "swing" of the vertex about its original position.
- M amplifies the effect of the swing.
- B affects the centerpoint of the vertex's swing. Set it to -M/2 for equal swing if you expect to cover T(x,y) such that you'll see its full range.

### WorldSpaceVertexOffsetMap

Because the material may be applied to multiple instances of an object at different world locations, it would look strange if all the instances were displaced in exactly the same way. The WorldSpaceVertexOffsetMap adds an additional modification to the displacements of the vertices of an object at a given world position. In addition, this map allows each vertex to be affected by a different position in the VertexDisplaceMap, rather than just the (0,0) point.

The texture map for WorldSpaceVertexOffsetMap is an RGB color map.

If the vertex is at global position X,Z (the Y position is ignored), then, after the texture scale and offset are applied, the texture's value is R, G, B (each within the range \[0,1\]). These values have the following effect on the displacement:

- The R channel is the offset added to x for the VertexDisplaceMap formula above.
- The G channel is the offset added to y for the VertexDisplaceMap formula above.

## Examples

Froox shows how the displace maps affect how the leaves in palm trees are shaped. Note that he is using a constantly bouncing LERP from 0 to 1 to simulate the effect of wind.

EmbedVideo is missing a required parameter.

## See Also

- [Component:PBS\_Metallic](https://wiki.resonite.com/Component:PBS_Metallic "Component:PBS Metallic")

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_DisplaceMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_DisplaceMetallic&oldid=105844](https://wiki.resonite.com/index.php?title=Component:PBS_DisplaceMetallic&oldid=105844)"

Contents