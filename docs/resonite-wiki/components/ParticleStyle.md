# Component:ParticleStyle

> Source: https://wiki.resonite.com/Component:ParticleStyle

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6b/Particlestyle.png/510px-Particlestyle.png)](https://wiki.resonite.com/File:Particlestyle.png) **Particle Style** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A **Particle Style** defines the visual appearance and behavior for a [ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Renderer` | **[IParticleRenderer](https://wiki.resonite.com/Type:IParticleRenderer "Type:IParticleRenderer")** | How to render the particles for systems this is assigned to. |
| `Modules` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IParticleSystemSubsystem](https://wiki.resonite.com/Type:IParticleSystemSubsystem "Type:IParticleSystemSubsystem")** | A list of modules to influence how the particle system looks and behaves. |
| `UseSystemLocalScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether particles should rely on the particle system's simulation space for scale. |
| `ParticleScaleMode` | **[ScaleMultiplierMode](https://wiki.resonite.com/Type:ScaleMultiplierMode "Type:ScaleMultiplierMode")** | How to scale particles during simulation for this style. |
| `UseSystemLocalRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether particles should rely on the particle system's simulation space for rotation. |

Fields
Collapse

## Usage

Used with a [ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem") to create the visuals and behavior for particles. multiple `Modules` can be used to make a variety of effects. Ranging from wind, laser dust swirling after firing, beat visualizers, element bending, and even accretion disks from black holes, the possibilities are endless.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleStyle&oldid=98789](https://wiki.resonite.com/index.php?title=Component:ParticleStyle&oldid=98789)"

Contents