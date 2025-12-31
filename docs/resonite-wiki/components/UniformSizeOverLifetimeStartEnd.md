# Component:UniformSizeOverLifetimeStartEnd

> Source: https://wiki.resonite.com/Component:UniformSizeOverLifetimeStartEnd

Collapse **Component image**

[File:UniformSizeOverLifetimeStartEndComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=UniformSizeOverLifetimeStartEndComponent.png "File:UniformSizeOverLifetimeStartEndComponent.png") **Uniform Size Over Lifetime Start End** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UniformSizeOverLifetimeStartEnd** component makes particles in a particle system start with a size and lerp towards an end size over their lifetime.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `StartSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size that particles have when starting or being born. |
| `EndSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size that particles go towards as their lifetime decreases. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:UniformSizeConstantInitializer](https://wiki.resonite.com/Component:UniformSizeConstantInitializer "Component:UniformSizeConstantInitializer") \\* Component:UniformSizeOverLifetimeStartEnd
- [Component:UniformSizeRangeInitializer](https://wiki.resonite.com/Component:UniformSizeRangeInitializer "Component:UniformSizeRangeInitializer")
- [Component:UniformSizeSineMultiplier](https://wiki.resonite.com/Component:UniformSizeSineMultiplier "Component:UniformSizeSineMultiplier")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UniformSizeOverLifetimeStartEnd&oldid=96079](https://wiki.resonite.com/index.php?title=Component:UniformSizeOverLifetimeStartEnd&oldid=96079)"

Contents