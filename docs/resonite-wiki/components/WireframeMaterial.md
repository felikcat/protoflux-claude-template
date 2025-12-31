# Component:WireframeMaterial

> Source: https://wiki.resonite.com/Component:WireframeMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:WireframeMaterial&diff=105882) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/WireframeMaterialComponent.png/510px-WireframeMaterialComponent.png)](https://wiki.resonite.com/File:WireframeMaterialComponent.png) **Wireframe Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Wireframe material is a material that can be used to see the edges of the polygons in a mesh. This does not show the polygons of a text renderer.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the thickness of the lines in the polygons |
| `ScreenSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the thickness should stay constant in width on the screen regardless of distance |
| `LineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color of this material's lines |
| `FillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color that should fill the center of each polygon. |
| `InnerLineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the lines on the inner frensel. |
| `InnerFillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the fill in the inner frensel. |
| `UseFresnel` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the frensel effect with the normal and inner line and fill colors. |
| `LineFarColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what the color of the lines should be when this material is rendered further away zbuffer wise. |
| `FillFarColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what the color of the fill should be when this material is rendered further away zbuffer wise. |
| `InnerLineFarColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what the color of the lines on the inner frensel should be when this material is rendered further away zbuffer wise. |
| `InnerFillFarColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what the color of the fill on the inner frensel should be when this material is rendered further away zbuffer wise. |
| `Exp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What exponent to raise colors to. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to debug data for. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |
| `DoubleSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to render this material on both sides. |
| `OffsetFactor` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer, based on the polygon's slope relative to the camera (i.e. polygons parallel to the camera will not be affected by this).[\[1\]](https://wiki.resonite.com/Component:WireframeMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `OffsetUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this material should be pushed forwards or backwards on the depth buffer (regardless of the polygon's slope relative to the camera), in units equal to the smallest possible difference for the rendering device being used.[\[1\]](https://wiki.resonite.com/Component:WireframeMaterial#cite_note-Material_OffsetFactor/Units_Desc-1) |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `_regular` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `_regularDoubleSided` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | [Template:Material regularDoubleSided](https://wiki.resonite.com/index.php?title=Template:Material_regularDoubleSided&action=edit&redlink=1 "Template:Material regularDoubleSided (page does not exist)") |

Fields
Collapse

## Usage

This is useful for debugging or making retro scenes. Simply apply this material to any skinned or mesh renderer's material slot to see that material assignment render this material style.

## Examples

## See Also

1. ↑ [Jump up to: 1.0](https://wiki.resonite.com/Component:WireframeMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-0)[1.1](https://wiki.resonite.com/Component:WireframeMaterial#cite_ref-Material_OffsetFactor/Units_Desc_1-1)[https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html](https://docs.unity3d.com/6000.2/Documentation/Manual/SL-Offset.html)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WireframeMaterial&oldid=105882](https://wiki.resonite.com/index.php?title=Component:WireframeMaterial&oldid=105882)"

Contents