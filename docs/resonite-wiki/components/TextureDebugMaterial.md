# Component:TextureDebugMaterial

> Source: https://wiki.resonite.com/Component:TextureDebugMaterial

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2c/TextureDebugMaterialComponent.png/510px-TextureDebugMaterialComponent.png)](https://wiki.resonite.com/File:TextureDebugMaterialComponent.png) **Texture Debug Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureDebugMaterial** component shows a grayscale of a texture channel. Used for debugging.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to debug data for. |
| `TextureChannel` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The channel to display from `Texture` as the surface. |

Fields
Collapse

## Usage

Attach to a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") with a mesh to view what this material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Color Splat Materials](https://wiki.resonite.com/Color_Splat_Materials "Color Splat Materials")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureDebugMaterial&oldid=105873](https://wiki.resonite.com/index.php?title=Component:TextureDebugMaterial&oldid=105873)"

Contents