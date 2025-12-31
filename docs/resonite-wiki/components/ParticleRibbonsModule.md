# Component:ParticleRibbonsModule

> Source: https://wiki.resonite.com/Component:ParticleRibbonsModule

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/80/ParticleRibbonsModuleComponent.png/510px-ParticleRibbonsModuleComponent.png)](https://wiki.resonite.com/File:ParticleRibbonsModuleComponent.png) **Particle Ribbons Module** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParticleRibbonsModule** component makes it to where a particle system will have ribbons that connect particles based on distance and other factors.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to give the ribbons |
| `TextureMode` | **[TrailTextureMode](https://wiki.resonite.com/index.php?title=Type:TrailTextureMode&action=edit&redlink=1 "Type:TrailTextureMode (page does not exist)")** | How to handle viewing the texture specified on the ribbons. |
| `MotionVectorMode` | **[MotionVectorMode](https://wiki.resonite.com/Type:MotionVectorMode "Type:MotionVectorMode")** | How to handle the rendering of ribbons in regards to motion vectors. |
| `GenerateLightingData` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to generate lighting data for the ribbons. |
| `RibbonPointRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many of the particles should be ribbons. |
| `Distribution` | **[ParticleFollowerDistribution](https://wiki.resonite.com/index.php?title=Type:ParticleFollowerDistribution&action=edit&redlink=1 "Type:ParticleFollowerDistribution (page does not exist)")** | How to distribute the ribbon followers. |
| `MaxRibbonPoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The max amount of ribbon points there should be. |
| `InterweavedRibbonCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of long particle-interconnected ribbons there can be, essentially multiple ribbons rather than one ribbon line. |
| `UseParticleColor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the color of particles the ribbons are following. |
| `UseParticleSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the size of particles the ribbons should follow. |
| `ShuffleInterweavedRibbons` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Randomly moves interweaved ribbon groups to new particles when they are generated. |
| `SizeInheritanceMode` | **[UniformSizeMode](https://wiki.resonite.com/index.php?title=Type:UniformSizeMode&action=edit&redlink=1 "Type:UniformSizeMode (page does not exist)")** | How to inherit the size of the particles the ribbons are following. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- Component:ParticleRibbonsModule
- [Component:RibbonColorConstantInitializer](https://wiki.resonite.com/Component:RibbonColorConstantInitializer "Component:RibbonColorConstantInitializer")
- [Component:RibbonColorRangeInitializer](https://wiki.resonite.com/Component:RibbonColorRangeInitializer "Component:RibbonColorRangeInitializer")
- [Component:RibbonFollowerColorConstantInitializer](https://wiki.resonite.com/Component:RibbonFollowerColorConstantInitializer "Component:RibbonFollowerColorConstantInitializer")
- [Component:RibbonFollowerColorRangeInitializer](https://wiki.resonite.com/Component:RibbonFollowerColorRangeInitializer "Component:RibbonFollowerColorRangeInitializer")
- [Component:RibbonFollowerWidthConstantInitializer](https://wiki.resonite.com/Component:RibbonFollowerWidthConstantInitializer "Component:RibbonFollowerWidthConstantInitializer")
- [Component:RibbonFollowerWidthRangeInitializer](https://wiki.resonite.com/Component:RibbonFollowerWidthRangeInitializer "Component:RibbonFollowerWidthRangeInitializer")
- [Component:RibbonWidthConstantInitializer](https://wiki.resonite.com/Component:RibbonWidthConstantInitializer "Component:RibbonWidthConstantInitializer")
- [Component:RibbonWidthRangeInitializer](https://wiki.resonite.com/Component:RibbonWidthRangeInitializer "Component:RibbonWidthRangeInitializer")
- [Component:SequenceRibbonSplitter](https://wiki.resonite.com/Component:SequenceRibbonSplitter "Component:SequenceRibbonSplitter")
- [Component:TimeProximityRibbonSplitter](https://wiki.resonite.com/Component:TimeProximityRibbonSplitter "Component:TimeProximityRibbonSplitter")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleRibbonsModule&oldid=105436](https://wiki.resonite.com/index.php?title=Component:ParticleRibbonsModule&oldid=105436)"

Contents