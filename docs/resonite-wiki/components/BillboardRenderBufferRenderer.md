# Component:BillboardRenderBufferRenderer

> Source: https://wiki.resonite.com/Component:BillboardRenderBufferRenderer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/41/BillboardRenderBufferRendererComponent.png/510px-BillboardRenderBufferRendererComponent.png)](https://wiki.resonite.com/File:BillboardRenderBufferRendererComponent.png) **Billboard Render Buffer Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BillboardRenderBufferRenderer** component is used as a debug component to determine the states of [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") buffers during the simulation process.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Buffer` | **[PointRenderBuffer](https://wiki.resonite.com/index.php?title=Type:PointRenderBuffer&action=edit&redlink=1 "Type:PointRenderBuffer (page does not exist)")** | The renderer to render point buffers. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to render this with. |
| `Alignment` | **[BillboardRenderBufferRenderer.BillboardAlignment](https://wiki.resonite.com/Component:BillboardRenderBufferRenderer#BillboardAlignment)** | How to align the particles. |
| `MotionVectorMode` | **[MotionVectorMode](https://wiki.resonite.com/Type:MotionVectorMode "Type:MotionVectorMode")** | How to render the object motion vectors. |
| `MinBillboardScreenSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum size of particles rendered. |
| `MaxBillboardScreenSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum size of particles rendered. |

Fields
Collapse

## Usage

Used in debugging [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

## Examples

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BillboardRenderBufferRenderer&oldid=106510](https://wiki.resonite.com/index.php?title=Component:BillboardRenderBufferRenderer&oldid=106510)"

Contents