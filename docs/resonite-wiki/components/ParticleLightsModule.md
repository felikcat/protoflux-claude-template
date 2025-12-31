# Component:ParticleLightsModule

> Source: https://wiki.resonite.com/Component:ParticleLightsModule

Collapse **Component image**

[File:ParticleLightsModuleComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ParticleLightsModuleComponent.png "File:ParticleLightsModuleComponent.png") **Particle Lights Module** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParticleLightsModule** makes a particle system create lights every so often for emitted particles that follow the particle they're assigned to.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TemplateLight` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Light](https://wiki.resonite.com/Component:Light "Component:Light") >** | The light to use as a template. |
| `LightsRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many lights as a percentage there should be from a 0 to 1 range. |
| `Distribution` | **[ParticleFollowerDistribution](https://wiki.resonite.com/index.php?title=Type:ParticleFollowerDistribution&action=edit&redlink=1 "Type:ParticleFollowerDistribution (page does not exist)")** | How to distribute the lights among the particles being emitted. |
| `MaxLights` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum number of lights that the particle system can have. |
| `MultiplyColorByParticle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to multiply the color of the lights by the color of the particle it is attached to. |
| `MultiplyIntensityByAlpha` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to multiply the intensity of the lights by the alpha channel of the color of the particle it is attached to. |
| `MultiplyRangeBySize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to multiply the range of the light based on the size of the particle it is attached to. |
| `AngleMultiplier` | **[AngleMultiplier](https://wiki.resonite.com/index.php?title=Type:AngleMultiplier&action=edit&redlink=1 "Type:AngleMultiplier (page does not exist)")** | How to influence the angle of the light based on the angle of the particle it is following. |
| `RangeMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the range of the light. |
| `IntensityMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to amplify the intensity of the light. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleLightsModule&oldid=97660](https://wiki.resonite.com/index.php?title=Component:ParticleLightsModule&oldid=97660)"

Contents