# Component:DepthProjectionMaterial

> Source: https://wiki.resonite.com/Component:DepthProjectionMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DepthProjectionMaterial&diff=105822) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ee/DepthProjectionMaterialComponent.png/510px-DepthProjectionMaterialComponent.png)](https://wiki.resonite.com/File:DepthProjectionMaterialComponent.png) **Depth Projection Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DepthProjectionMaterial** is commonly used when importing depth videos and acts as a material that displaces vertices in 3D.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Color` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The surface color texture of the material. |
| `Depth` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | the texture used to displace vertices based on intensity. |
| `DepthEncoding` | **[DepthEncoding](https://wiki.resonite.com/Type:DepthEncoding "Type:DepthEncoding")** | How the depth data is encoded into `Depth` |
| `ColorTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the texture uv offset of `Color`. |
| `ColorTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the texture uv scale of `Color`. |
| `DepthTextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the texture uv offset of `Depth`. |
| `DepthTextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the texture uv scale of `Depth`. |
| `DepthFrom` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum depth distance. |
| `DepthTo` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum depth distance. |
| `FieldOfView` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the field of view of the `Depth` data. |
| `NearClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the near clip of the `Depth` data. |
| `FarClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the far clip of the `Depth` data. |
| `DiscardThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how strong the depth data can be till its cut off. |
| `DiscardOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to offset the `DiscardThreshold`. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `ZWrite` | **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | whether this material should respect the distance it is from the camera. |

Fields
Collapse

## Usage

The material uses a file that has a greyscale video (representing depth at each pixel) and a normal color video in order to "overlay" the color info on top of the 3D distortion created by the greyscale input. There are texture2D slots for depth and color, meaning two separate files could be used given the DepthTextureOffset property is set to 0.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DepthProjectionMaterial&oldid=105822](https://wiki.resonite.com/index.php?title=Component:DepthProjectionMaterial&oldid=105822)"

Contents