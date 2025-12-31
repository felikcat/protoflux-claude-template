# Component:TrailsRenderBufferRenderer

> Source: https://wiki.resonite.com/Component:TrailsRenderBufferRenderer

Collapse **Component image**

[File:TrailsRenderBufferRendererComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=TrailsRenderBufferRendererComponent.png "File:TrailsRenderBufferRendererComponent.png") **Trails Render Buffer Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TrailsRenderBufferRenderer** component is mainly a debug component to show the allocation of rendering buffers for particles in the form of colors. This relies on the specific implementation of [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Buffer` | **[TrailsRenderBuffer](https://wiki.resonite.com/index.php?title=Type:TrailsRenderBuffer&action=edit&redlink=1 "Type:TrailsRenderBuffer (page does not exist)")** | The trails renderer module to get buffer data from. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to use for rendering. |
| `TextureMode` | **[TrailTextureMode](https://wiki.resonite.com/index.php?title=Type:TrailTextureMode&action=edit&redlink=1 "Type:TrailTextureMode (page does not exist)")** | The texture mode to use for rendering. |
| `MotionVectorMode` | **[MotionVectorMode](https://wiki.resonite.com/Type:MotionVectorMode "Type:MotionVectorMode")** | The motion vector mode for rendering from a camera. |
| `GenerateLightingData` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to generate lighting data for trail rendering. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TrailsRenderBufferRenderer&oldid=106598](https://wiki.resonite.com/index.php?title=Component:TrailsRenderBufferRenderer&oldid=106598)"

Contents