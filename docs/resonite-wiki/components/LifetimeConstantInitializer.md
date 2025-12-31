# Component:LifetimeConstantInitializer

> Source: https://wiki.resonite.com/Component:LifetimeConstantInitializer

Collapse **Component image**

[File:LifetimeConstantInitializerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LifetimeConstantInitializerComponent.png "File:LifetimeConstantInitializerComponent.png") **Lifetime Constant Initializer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LifeTimeConstantInitializer** component makes all particles in a particle system start with a lifetime/duration of `Value`.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lifetime all particles should start with in the particle system. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LifetimeConstantInitializer&oldid=96095](https://wiki.resonite.com/index.php?title=Component:LifetimeConstantInitializer&oldid=96095)"

Contents