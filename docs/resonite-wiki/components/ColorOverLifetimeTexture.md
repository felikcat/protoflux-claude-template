# Component:ColorOverLifetimeTexture

> Source: https://wiki.resonite.com/Component:ColorOverLifetimeTexture

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c0/ColorOverLifetimeTextureComponent.png/510px-ColorOverLifetimeTextureComponent.png)](https://wiki.resonite.com/File:ColorOverLifetimeTextureComponent.png) **Color Over Lifetime Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorOverLifetimeTexture** component samples a texture during life time along the X axis to get the color that a Particle should be.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to sample along the X axis based on Lifetime normalized to get a color for particles. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

## See Also

- [Component:ColorOverLifetimeStartEnd](https://wiki.resonite.com/Component:ColorOverLifetimeStartEnd "Component:ColorOverLifetimeStartEnd")
- [Component:ColorHSV OverLifetimeStartEnd](https://wiki.resonite.com/Component:ColorHSV_OverLifetimeStartEnd "Component:ColorHSV OverLifetimeStartEnd")
- Component:ColorOverLifetimeTexture
- [Component:AlphaOverLifetimeLinearGradient](https://wiki.resonite.com/Component:AlphaOverLifetimeLinearGradient "Component:AlphaOverLifetimeLinearGradient")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorOverLifetimeTexture&oldid=96024](https://wiki.resonite.com/index.php?title=Component:ColorOverLifetimeTexture&oldid=96024)"

Contents