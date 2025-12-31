# Component:UVW ProceduralTexture3D

> Source: https://wiki.resonite.com/Component:UVW_ProceduralTexture3D

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UVW_ProceduralTexture3D&diff=113619) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/UVW_ProceduralTexture3DComponent.png/510px-UVW_ProceduralTexture3DComponent.png)](https://wiki.resonite.com/File:UVW_ProceduralTexture3DComponent.png) **UVW Procedural Texture 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UVWProceduralTexture3D** component is used to create a default RGB cube that any XYZ coordinate corresponds to the same RGB color, as a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D"). This works as long as if `ValueOffset` is left at 0 and `ValueMultiplier` is left at 1. This means if it is plugged into a [LUT Material](https://wiki.resonite.com/Component:LUT_Material "Component:LUT Material"), it will not modify the colors seen through the material.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the X axis. this goes into affect when X values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Y axis. this goes into affect when Y values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeW` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Z axis. this goes into affect when Z values are outside of the range \[0.0 to 1.0\]. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile to use for this texture's rendering. |
| `Size` | **[Int3](https://wiki.resonite.com/Type:Int3 "Type:Int3")** | The size of the procedural texture in pixels. |
| `Format` | **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | TextureFormat describes how Texture's pixel are stored in the VRAM. |
| `ValueOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to add to the colors in the cube by, which shifts all colors towards the +X,+Y,+Z direction. |
| `ValueMultiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to multiply the colors in the cube by, which scales all colors towards the +X,+Y,+Z direction. |

Fields
Collapse

## Usage

Attach to a slot and insert into either a [VolumeUnlitMaterial](https://wiki.resonite.com/Component:VolumeUnlitMaterial "Component:VolumeUnlitMaterial") or a [LUT Material](https://wiki.resonite.com/Component:LUT_Material "Component:LUT Material") to view what it looks like or how it modifies colors.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UVW\_ProceduralTexture3D&oldid=113619](https://wiki.resonite.com/index.php?title=Component:UVW_ProceduralTexture3D&oldid=113619)"

Contents