# Component:FurMaterial

> Source: https://wiki.resonite.com/Component:FurMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FurMaterial&diff=105827) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/88/FurMaterialComponent.png/510px-FurMaterialComponent.png)](https://wiki.resonite.com/File:FurMaterialComponent.png) **Fur Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FurMaterial** component is used to make multi layered geometry out of a mesh's original geometry that has a specified distance between layers. The number of layers is a constant 20. Combined with a map to create holes in the layers via alpha, this creates the illusion of depth and fur like properties. The geometry layers are instanced on the GPU.

Some players have reported lag when using Fur materials. This is due to either using too large of a texture, or due to an issue called Overdraw.

Overdraw is caused when the GPU generates pixels for a layer for where it appears on the screen in a stage in rendering called "Rasterization" when it is done, it renders the next layer, and has to draw that on top of the already drawn layer pixels. The drawing on top for the next 19 layers is called Overdraw.

This means that if a user looks very closely at a fur shader, or the shader covers their entire screen while all layers are in front of the camera, it will lag intensely. This is because the game is doing 20 drawing cycles on every pixel. Causing significant lag.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The surface color texture of the material. |
| `SpecularColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Specular Tint. Behaves like PBS Specular Tinting |
| `Shininess` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Behaves like PBS Smoothness |
| `Gloss` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Reflection Intensity. |
| `RimColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Rim Lighting Color |
| `RimPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Rim Lighting Power |
| `FurLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Length of the fur. Always applied in the force direction. |
| `FurHardness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How Stiff the fur is. Biases fur to point in the mesh normal direction instead of the force direction. |
| `FurThinness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many times to re-iterate the fur noise map. Behaves similarly to texture scaling. |
| `FurShading` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much fake shading should be applied to the fur. |
| `FurColoring` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the color of the fur should take precedent over shading. |
| `Base` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Albedo Texture. Alpha is Heightmap |
| `NormalMap` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The normal map is used as a way to change the appearance of a surface when shined on by lights, to give the illusion of a raised surface. |
| `Noise` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Noise texture. This should always be on the alpha channel. This determines the pattern of the fur. |
| `TextureScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up or down the different texture maps. |
| `TextureOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to shift around the position of the different texture maps. |
| `AlphaCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If `BlendMode` is set to cutout, discard rendering of pixels for the surface that fall below this alpha threshold. |
| `ForceGlobal` | **[Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4")** | The amount of displacement to apply in the world coordinate system. The **W** value corresponds to a proportional affinity to point towards world origin. |
| `ForceLocal` | **[Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4")** | The amount of displacement to apply in the object's local coordinate system. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Usage

Insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") with a mesh to view what the material looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FurMaterial&oldid=105827](https://wiki.resonite.com/index.php?title=Component:FurMaterial&oldid=105827)"

Contents