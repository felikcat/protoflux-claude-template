# Component:BillboardParticleRenderer

> Source: https://wiki.resonite.com/Component:BillboardParticleRenderer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/BillboardParticleRendererComponent.png/510px-BillboardParticleRendererComponent.png)](https://wiki.resonite.com/File:BillboardParticleRendererComponent.png) **Billboard Particle Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BillboardParticleRenderer** component is a rendering style component for Particle systems that give them the default square tile based particles.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to use to render the particles. |
| `Alignment` | **[BillboardRenderBufferRenderer.BillboardAlignment](https://wiki.resonite.com/Component:BillboardRenderBufferRenderer#BillboardAlignment "Component:BillboardRenderBufferRenderer")** | How to align the particles. |
| `MinBillboardScreenSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum size a particle can be on the screen. |
| `MaxBillboardScreenSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum size a particle can be on the screen. |
| `MotionVectorMode` | **[MotionVectorMode](https://wiki.resonite.com/Type:MotionVectorMode "Type:MotionVectorMode")** | How to handle rendering particles when it comes to their motion vectors. |

Fields
Collapse

## Usage

Attach to a slot, add to the renderer slot in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Making a simple cloud of particles or fire or any other Particle effect.

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BillboardParticleRenderer&oldid=98197](https://wiki.resonite.com/index.php?title=Component:BillboardParticleRenderer&oldid=98197)"

Contents