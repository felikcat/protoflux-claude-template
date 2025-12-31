# Component:TextUnlitMaterial

> Source: https://wiki.resonite.com/Component:TextUnlitMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TextUnlitMaterial&diff=105872) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fd/TextUnlitMaterialComponent.png/510px-TextUnlitMaterialComponent.png)](https://wiki.resonite.com/File:TextUnlitMaterialComponent.png) **Text Unlit Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextUnlitMaterial** component is a material used to render text glyphs. It does so via meshes that automatically generates UV maps that map to each character on a font map. Such as [Component:Text](https://wiki.resonite.com/Component:Text "Component:Text") and [Component:TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `FontAtlas` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The font to render. |
| `TintColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What color to tint the projected image. |
| `OutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the outline around the mesh. |
| `BackgroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of behind each text glyph |
| `AutoBackgroundColor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to automatically generate the background text color. |
| `GlyphRenderMethod` | **[GlyphRenderMethod](https://wiki.resonite.com/index.php?title=Type:GlyphRenderMethod&action=edit&redlink=1 "Type:GlyphRenderMethod (page does not exist)")** | How to render each glyph or text character. |
| `PixelRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Sets the distance field range in output pixels. |
| `FaceDilate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fat to make the letters like bolding them. |
| `OutlineThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the outline on text for colored outlines. |
| `FaceSoftness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much blurring to do on the edges of the text. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `Sidedness` | **[Sidedness](https://wiki.resonite.com/Type:Sidedness "Type:Sidedness")** | Render on both sides of the mesh, front, or back. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `ZTest` | **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | Determines whether this object should render when it is in front of or behind other objects that respect depth from the camera |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:TextUnlitMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:TextUnlitMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in rendering [Component:TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer") and [Component:Text](https://wiki.resonite.com/Component:Text "Component:Text")

## See Also

- [Component:TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")
- [Component:UI\_TextUnlitMaterial](https://wiki.resonite.com/Component:UI_TextUnlitMaterial "Component:UI TextUnlitMaterial")

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:TextUnlitMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:TextUnlitMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextUnlitMaterial&oldid=105872](https://wiki.resonite.com/index.php?title=Component:TextUnlitMaterial&oldid=105872)"

Contents