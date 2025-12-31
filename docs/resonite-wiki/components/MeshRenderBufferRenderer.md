# Component:MeshRenderBufferRenderer

> Source: https://wiki.resonite.com/Component:MeshRenderBufferRenderer

Collapse **Component image**

[File:MeshRenderBufferRendererComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=MeshRenderBufferRendererComponent.png "File:MeshRenderBufferRendererComponent.png") **Mesh Render Buffer Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshRenderBufferRenderer** component is used to render point buffers for normal particles as meshes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Buffer` | **[PointRenderBuffer](https://wiki.resonite.com/index.php?title=Type:PointRenderBuffer&action=edit&redlink=1 "Type:PointRenderBuffer (page does not exist)")** | The Buffer to render as meshes. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to render on the meshes. |
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to render. |
| `Alignment` | **[MeshRenderBufferRenderer.MeshAlignment](https://wiki.resonite.com/Component:MeshRenderBufferRenderer#MeshAlignment)** | How to align the meshes rendered using orientation and camera position. |

Fields
Collapse

## MeshAlignment

| Name | Value | Description |
| --- | --- | --- |
| `View` | 0 | Orient the meshes towards the camera. |
| `Facing` | 1 | Orient the meshes based on particle direction. |
| `Local` | 2 | Orient the particles based on local transformation. |
| `Global` | 3 | Orient the particles based on global transformation. |

Values

## Usage

Used with [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust").

## Examples

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshRenderBufferRenderer&oldid=105329](https://wiki.resonite.com/index.php?title=Component:MeshRenderBufferRenderer&oldid=105329)"

Contents