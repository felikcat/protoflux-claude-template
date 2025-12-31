# Component:SimplexTexture

> Source: https://wiki.resonite.com/Component:SimplexTexture

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SimplexTexture&diff=98064) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c7/SimplexTextureComponent.png/510px-SimplexTextureComponent.png)](https://wiki.resonite.com/File:SimplexTextureComponent.png) **Simplex Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SimplexTexture** component is used to generate procedural noise to use in any [material](https://wiki.resonite.com/Material "Material").

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
| `MipmapBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether to see lower resolution versions of the texture closer up or not (MipMaps). |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile to use for this texture's rendering. |
| `Size` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The size of the procedural texture in pixels. |
| `Mipmaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enable the rendering of mipmaps, which are lower res textures at further distances from the camera to improve performance. |
| `Format` | **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | TextureFormat describes how Texture's pixel are stored in the VRAM. |
| `Offset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift the procedural noise. |
| `Scale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | scales the pattern up or down inside the image. |
| `Background` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The background color of the noise. |
| `Foreground` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the noise itself. |
| `Use3D` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow `ZOffset` to affect the texture, and generates 3D noise. |
| `ZOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset in the 3D noise, which takes a slice of the 3D noise for the texture. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeTexture:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | BakeTexture first generates a [Component:StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D") that is the same as this procedural texture. The resulting static texture replaces every reference to the original procedural texture. Lastly the original procedural texture is deleted. |

Triggers
Collapse

## Usage

Insert into any [material](https://wiki.resonite.com/Material "Material") to view what this texture looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SimplexTexture&oldid=98064](https://wiki.resonite.com/index.php?title=Component:SimplexTexture&oldid=98064)"

Contents