# Component:CheckerboardCubemap

> Source: https://wiki.resonite.com/Component:CheckerboardCubemap

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CheckerboardCubemap&diff=93420) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/92/CheckerboardCubemapComponent.png/510px-CheckerboardCubemapComponent.png)](https://wiki.resonite.com/File:CheckerboardCubemapComponent.png) **Checkerboard Cubemap** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CheckerboardCubemap** component procedurally generates a cubemap for [Projection 360 Materials](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material") that is a checkerboard with different pairs of colors for each of the 6 sides.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `MipmapBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether to see lower resolution versions of the texture closer up or not (MipMaps). |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile to use for this texture's rendering. |
| `Size` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The size of each side of the cubemap in pixels. |
| `Mipmaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enable the rendering of mipmaps, which are lower res textures at further distances from the camera to improve performance. |
| `Format` | **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | TextureFormat describes how Texture's pixel are stored in the VRAM. |
| `CheckerSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The size in pixels for 1 square of the checkerboard pattern. |
| `PosX_Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 for the Positive X direction image's checkerboard pattern. |
| `PosX_Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 for the Positive X direction image's checkerboard pattern. |
| `NegX_Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 for the Negative X direction image's checkerboard pattern. |
| `NegX_Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 for the Negative X direction image's checkerboard pattern. |
| `PosY_Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 for the Positive Y direction image's checkerboard pattern. |
| `PosY_Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 for the Positive Y direction image's checkerboard pattern. |
| `NegY_Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 for the Negative Y direction image's checkerboard pattern. |
| `NegY_Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 for the Negative Y direction image's checkerboard pattern. |
| `PosZ_Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 for the Positive Z direction image's checkerboard pattern. |
| `PosZ_Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 for the Positive Z direction image's checkerboard pattern. |
| `NegZ_Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 1 for the Negative Z direction image's checkerboard pattern. |
| `NegZ_Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color 2 for the Negative Z direction image's checkerboard pattern. |

Fields
Collapse

## Usage

Put into the `CubeMap` field of a [Projection 360 Materials](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material") to view what the skybox would look like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Usually used for debugging, or for a fever dream chess world.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CheckerboardCubemap&oldid=93420](https://wiki.resonite.com/index.php?title=Component:CheckerboardCubemap&oldid=93420)"

Contents