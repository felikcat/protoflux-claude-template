# Component:PBS DistanceLerpMetallic

> Source: https://wiki.resonite.com/Component:PBS_DistanceLerpMetallic

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/PBS_DistanceLerpMetallicComponent.png/510px-PBS_DistanceLerpMetallicComponent.png)](https://wiki.resonite.com/File:PBS_DistanceLerpMetallicComponent.png) **PBS Distance Lerp Metallic** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Works on meshes with dense vertices. Can apply tint based on distance to specified points, and also displaces the vertices in the mesh based on distance to specified points (possibly towards/away from the point).

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
| `GridSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | [Template:Material GridSize](https://wiki.resonite.com/index.php?title=Template:Material_GridSize&action=edit&redlink=1 "Template:Material GridSize (page does not exist)") |
| `GridOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | [Template:Material GridOffset](https://wiki.resonite.com/index.php?title=Template:Material_GridOffset&action=edit&redlink=1 "Template:Material GridOffset (page does not exist)") |
| `DisplaceFrom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material DisplaceFrom](https://wiki.resonite.com/index.php?title=Template:Material_DisplaceFrom&action=edit&redlink=1 "Template:Material DisplaceFrom (page does not exist)") |
| `DisplaceTo` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material DisplaceTo](https://wiki.resonite.com/index.php?title=Template:Material_DisplaceTo&action=edit&redlink=1 "Template:Material DisplaceTo (page does not exist)") |
| `DisplaceMagnitudeFrom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material DisplaceMagnitudeFrom](https://wiki.resonite.com/index.php?title=Template:Material_DisplaceMagnitudeFrom&action=edit&redlink=1 "Template:Material DisplaceMagnitudeFrom (page does not exist)") |
| `DisplaceMagnitudeTo` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material DisplaceMagnitudeTo](https://wiki.resonite.com/index.php?title=Template:Material_DisplaceMagnitudeTo&action=edit&redlink=1 "Template:Material DisplaceMagnitudeTo (page does not exist)") |
| `EmissionFrom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material EmissionFrom](https://wiki.resonite.com/index.php?title=Template:Material_EmissionFrom&action=edit&redlink=1 "Template:Material EmissionFrom (page does not exist)") |
| `EmissionTo` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material EmissionTo](https://wiki.resonite.com/index.php?title=Template:Material_EmissionTo&action=edit&redlink=1 "Template:Material EmissionTo (page does not exist)") |
| `EmissionColorFrom` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | [Template:Material EmissionColorFrom](https://wiki.resonite.com/index.php?title=Template:Material_EmissionColorFrom&action=edit&redlink=1 "Template:Material EmissionColorFrom (page does not exist)") |
| `EmissionColorTo` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | [Template:Material EmissionColorTo](https://wiki.resonite.com/index.php?title=Template:Material_EmissionColorTo&action=edit&redlink=1 "Template:Material EmissionColorTo (page does not exist)") |
| `OverrideDisplacementDirection` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | [Template:Material OverrideDisplacementDirection](https://wiki.resonite.com/index.php?title=Template:Material_OverrideDisplacementDirection&action=edit&redlink=1 "Template:Material OverrideDisplacementDirection (page does not exist)") |
| `LocalSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to calculate `Distance` and `Point` in local space. |
| `Points` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Point](https://wiki.resonite.com/index.php?title=Type:Point&action=edit&redlink=1 "Type:Point (page does not exist)")** | A list of (global) positions and tints. The tint is applied to mesh vertices more or less depending on the mesh vertex's distance to the given point: larger distances means less tint. |
| `Culling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Whether to show the material on the front, back, or both sides |
| `Transparent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this should render transparent |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:PBS_DistanceLerpMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:PBS_DistanceLerpMetallic#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `Metallic` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much metallicness the surface should have if `MetallicMap` is not specified. |
| `Smoothness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much smoothness the surface should have if `MetallicMap` is not specified. |
| `MetallicMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | [Metallic Maps](https://wiki.resonite.com/Component:PBS_Metallic#Metallic_Maps "Component:PBS Metallic") |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_transparent` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Shader, Internal. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:PBS_DistanceLerpMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:PBS_DistanceLerpMetallic#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PBS\_DistanceLerpMetallic&oldid=105846](https://wiki.resonite.com/index.php?title=Component:PBS_DistanceLerpMetallic&oldid=105846)"

Contents