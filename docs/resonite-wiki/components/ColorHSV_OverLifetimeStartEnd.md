# Component:ColorHSV OverLifetimeStartEnd

> Source: https://wiki.resonite.com/Component:ColorHSV_OverLifetimeStartEnd

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8a/ColorHSV_OverLifetimeStartEndComponent.png/510px-ColorHSV_OverLifetimeStartEndComponent.png)](https://wiki.resonite.com/File:ColorHSV_OverLifetimeStartEndComponent.png) **Color HSV Over Lifetime Start End** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorHSV\_OverLifetimeStartEnd** component makes particles have an HSV value that lerps from start to end over the particle's lifetime.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `StartHue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting hue at birth of a particle. |
| `StartSaturation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting saturation at birth of a particle. |
| `StartValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting value at birth of a particle. |
| `EndHue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending hue at death of a particle. |
| `EndSaturation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending staturation at death of a particle. |
| `EndValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending value at death of a particle. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Type:Color](https://wiki.resonite.com/Type:Color "Type:Color")
- [Component:ColorOverLifetimeStartEnd](https://wiki.resonite.com/Component:ColorOverLifetimeStartEnd "Component:ColorOverLifetimeStartEnd")
- Component:ColorHSV OverLifetimeStartEnd
- [Component:ColorOverLifetimeTexture](https://wiki.resonite.com/Component:ColorOverLifetimeTexture "Component:ColorOverLifetimeTexture")
- [Component:AlphaOverLifetimeLinearGradient](https://wiki.resonite.com/Component:AlphaOverLifetimeLinearGradient "Component:AlphaOverLifetimeLinearGradient")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorHSV\_OverLifetimeStartEnd&oldid=96045](https://wiki.resonite.com/index.php?title=Component:ColorHSV_OverLifetimeStartEnd&oldid=96045)"

Contents