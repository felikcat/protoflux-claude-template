# Component:DebugMaterial

> Source: https://wiki.resonite.com/Component:DebugMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DebugMaterial&diff=105820) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/de/DebugMaterialComponent.png/510px-DebugMaterialComponent.png)](https://wiki.resonite.com/File:DebugMaterialComponent.png) **Debug Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugMaterial** component is used to display mesh data in the form of a color map.

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
| `Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale the positions of the displayed color data pixels. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to offset the positions of the displayed color data pixels. |
| `Visualize` | **[MeshData](https://wiki.resonite.com/Component:DebugMaterial#MeshData)** | What kind of data to visualize for the mesh. |
| `Normalize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enable keeping visualized mesh data within a 0-1 range for all color values. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Usage

## MeshData

_This article or section is a stub. You can help the Resonite wiki by expanding it._

| Name | Value | Description |
| --- | --- | --- |
| `Position` | 0 | Position of the mesh in world space. |
| `Color` | 1 | The vertex colors of the mesh |
| `ColorAlpha` | 2 | The alpha of the vertex colors of the mesh. |
| `Normals` | 3 | The polygon normal shading data of the mesh. |
| `Tangents` | 4 | the polygon tangent data of the mesh. |
| `TangentDir` | 5 | the polygon tangent direction data of the mesh. |
| `Bitangents` | 6 | the polygon Bi tangent data of the mesh. |
| `UV0s` | 7 | The first UV map data of the mesh |
| `UV1s` | 8 | The second UV map data of the mesh |
| `UV2s` | 9 | The third UV map data of the mesh |
| `UV3s` | 10 | The last UV map data of the mesh |

Values

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugMaterial&oldid=105820](https://wiki.resonite.com/index.php?title=Component:DebugMaterial&oldid=105820)"

Contents