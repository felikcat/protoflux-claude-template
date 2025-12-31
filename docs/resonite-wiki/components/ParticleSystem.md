# Component:ParticleSystem

> Source: https://wiki.resonite.com/Component:ParticleSystem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/85/ParticleSystemComponent.png/510px-ParticleSystemComponent.png)](https://wiki.resonite.com/File:ParticleSystemComponent.png) **Particle System** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The **ParticleSystem** component acts as the interface between a particle style and one or more particle emitter.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MaxParticleCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum particles controlled by this component that can exist at any given time. |
| `Style` | **[ParticleStyle](https://wiki.resonite.com/Component:ParticleStyle "Component:ParticleStyle")** | The ParticleStyle component that this component is using. |
| `SimulationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space the emitted particles will do calculations and physics under. (They are not actually placed under this slot, but they visually behave as though they are). |

Fields
Collapse

## Usage

With a particle system, multiple emitters can use the same source [ParticleStyle](https://wiki.resonite.com/Component:ParticleStyle "Component:ParticleStyle"). Alternatively, multiple ParticleSystems can be used with the same style but different simulation spaces to avoid the need for multiple style components. This is especially handy when properties of the style need to be dynamically changed as it can be done from a centralized location.

## Examples

## See also

- [Component:ParticleStyle](https://wiki.resonite.com/Component:ParticleStyle "Component:ParticleStyle")
- [Component:PointEmitter](https://wiki.resonite.com/Component:PointEmitter "Component:PointEmitter")
- [Component:CircleEmitter](https://wiki.resonite.com/Component:CircleEmitter "Component:CircleEmitter")
- [Component:SphereEmitter](https://wiki.resonite.com/Component:SphereEmitter "Component:SphereEmitter")
- [Component:CylinderEmitter](https://wiki.resonite.com/Component:CylinderEmitter "Component:CylinderEmitter")
- [Component:ConeEmitter](https://wiki.resonite.com/Component:ConeEmitter "Component:ConeEmitter")
- [Component:LineEmitter](https://wiki.resonite.com/Component:LineEmitter "Component:LineEmitter")
- [Component:BoxEmitter](https://wiki.resonite.com/Component:BoxEmitter "Component:BoxEmitter")
- [Component:SkinnedMeshEmitter](https://wiki.resonite.com/Component:SkinnedMeshEmitter "Component:SkinnedMeshEmitter")
- [Component:MeshEmitter](https://wiki.resonite.com/Component:MeshEmitter "Component:MeshEmitter")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleSystem&oldid=108400](https://wiki.resonite.com/index.php?title=Component:ParticleSystem&oldid=108400)"

Contents