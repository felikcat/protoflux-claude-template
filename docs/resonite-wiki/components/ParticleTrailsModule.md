# Component:ParticleTrailsModule

> Source: https://wiki.resonite.com/Component:ParticleTrailsModule

Collapse **Component image**

[File:ParticleTrailsModuleComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ParticleTrailsModuleComponent.png "File:ParticleTrailsModuleComponent.png") **Particle Trails Module** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParticleTrailsModule** component allows particles to have trails with different properties. This can be added multiple times for different trail types.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material the particle trails should have. |
| `TextureMode` | **[TrailTextureMode](https://wiki.resonite.com/index.php?title=Type:TrailTextureMode&action=edit&redlink=1 "Type:TrailTextureMode (page does not exist)")** | How to handle the textures on trails. |
| `MotionVectorMode` | **[MotionVectorMode](https://wiki.resonite.com/Type:MotionVectorMode "Type:MotionVectorMode")** | How to handle rendering the trails when it comes to motion vectors. |
| `GenerateLightingData` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the trails have lighting data. |
| `TrailsRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many of the particles as a 0<->1 percentage should have trails |
| `Distribution` | **[ParticleFollowerDistribution](https://wiki.resonite.com/index.php?title=Type:ParticleFollowerDistribution&action=edit&redlink=1 "Type:ParticleFollowerDistribution (page does not exist)")** | How to distribute the followers for this module. |
| `MaxTrails` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum amount of trails the system can have of this particular trail type. |
| `SimulationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | What Transform space to simulate the trails for this module in? |
| `MinVertexDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum vertex distance between trail segments when generating trail geometry. |
| `TrailDiesWithParticle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the trail disappears instantly when the particle dies or not. |
| `ParticleColorInheritance` | **[TrailParticleInheritance](https://wiki.resonite.com/index.php?title=Type:TrailParticleInheritance&action=edit&redlink=1 "Type:TrailParticleInheritance (page does not exist)")** | How the trail inherits the color of the particle it's following. |
| `ParticleSizeInheritance` | **[TrailParticleInheritance](https://wiki.resonite.com/index.php?title=Type:TrailParticleInheritance&action=edit&redlink=1 "Type:TrailParticleInheritance (page does not exist)")** | How the trail inherits the size of the particle it's following. |
| `SizeInheritanceMode` | **[UniformSizeMode](https://wiki.resonite.com/index.php?title=Type:UniformSizeMode&action=edit&redlink=1 "Type:UniformSizeMode (page does not exist)")** | How the size the trail inherited from the particle it's followinh should be applied. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- Component:ParticleTrailsModule
- [Component:TrailColorConstantInitializer](https://wiki.resonite.com/Component:TrailColorConstantInitializer "Component:TrailColorConstantInitializer")
- [Component:TrailColorRangeInitializer](https://wiki.resonite.com/Component:TrailColorRangeInitializer "Component:TrailColorRangeInitializer")
- [Component:TrailLifetimeConstantInitializer](https://wiki.resonite.com/Component:TrailLifetimeConstantInitializer "Component:TrailLifetimeConstantInitializer")
- [Component:TrailLifetimeFromSizeInitializer](https://wiki.resonite.com/Component:TrailLifetimeFromSizeInitializer "Component:TrailLifetimeFromSizeInitializer")
- [Component:TrailLifetimeRangeInitializer](https://wiki.resonite.com/Component:TrailLifetimeRangeInitializer "Component:TrailLifetimeRangeInitializer")
- [Component:TrailWidthConstantInitializer](https://wiki.resonite.com/Component:TrailWidthConstantInitializer "Component:TrailWidthConstantInitializer")
- [Component:TrailWidthRangeInitializer](https://wiki.resonite.com/Component:TrailWidthRangeInitializer "Component:TrailWidthRangeInitializer")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleTrailsModule&oldid=96048](https://wiki.resonite.com/index.php?title=Component:ParticleTrailsModule&oldid=96048)"

Contents