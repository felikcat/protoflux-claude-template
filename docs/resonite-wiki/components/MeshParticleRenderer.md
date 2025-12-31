# Component:MeshParticleRenderer

> Source: https://wiki.resonite.com/Component:MeshParticleRenderer

Collapse **Component image**

[File:MeshParticleRendererComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=MeshParticleRendererComponent.png "File:MeshParticleRendererComponent.png") **Mesh Particle Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshParticleRenderer** component is a particle renderer that makes all particle instances in a particle system render as a specific mesh.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material the particles should have. |
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh object to GPU instance to all particle points and render. |
| `Alignment` | **[MeshRenderBufferRenderer.MeshAlignment](https://wiki.resonite.com/Component:MeshRenderBufferRenderer#MeshAlignment "Component:MeshRenderBufferRenderer")** | How to align the meshes with the particle transforms. |

Fields
Collapse

## Usage

Attach to a slot, add to the renderer slot in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Making a rock slide using actual rock meshes via Photon Dust.

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshParticleRenderer&oldid=98203](https://wiki.resonite.com/index.php?title=Component:MeshParticleRenderer&oldid=98203)"

Contents