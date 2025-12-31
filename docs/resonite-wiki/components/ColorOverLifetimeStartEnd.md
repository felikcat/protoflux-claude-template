# Component:ColorOverLifetimeStartEnd

> Source: https://wiki.resonite.com/Component:ColorOverLifetimeStartEnd

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ee/ColorOverLifetimeStartEndComponent.png/510px-ColorOverLifetimeStartEndComponent.png)](https://wiki.resonite.com/File:ColorOverLifetimeStartEndComponent.png) **Color Over Lifetime Start End** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorOverLifetimeStartEnd** component makes particles in a Particle system change color linearly over the duration of their lifetime.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `StartColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color particles should be when emitted. |
| `EndColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color particles should lerp towards over their lifetime and they will have this color right before they die. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

## See Also

- Component:ColorOverLifetimeStartEnd
- [Component:ColorHSV OverLifetimeStartEnd](https://wiki.resonite.com/Component:ColorHSV_OverLifetimeStartEnd "Component:ColorHSV OverLifetimeStartEnd")
- [Component:ColorOverLifetimeTexture](https://wiki.resonite.com/Component:ColorOverLifetimeTexture "Component:ColorOverLifetimeTexture")
- [Component:AlphaOverLifetimeLinearGradient](https://wiki.resonite.com/Component:AlphaOverLifetimeLinearGradient "Component:AlphaOverLifetimeLinearGradient")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorOverLifetimeStartEnd&oldid=97276](https://wiki.resonite.com/index.php?title=Component:ColorOverLifetimeStartEnd&oldid=97276)"

Contents