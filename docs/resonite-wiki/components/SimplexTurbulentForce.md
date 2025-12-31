# Component:SimplexTurbulentForce

> Source: https://wiki.resonite.com/Component:SimplexTurbulentForce

Collapse **Component image**

[File:SimplexTurbulentForceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SimplexTurbulentForceComponent.png "File:SimplexTurbulentForceComponent.png") **Simplex Turbulent Force** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SimplexTurbulentForce** component is used to make random noise throughout an entire particle system that affects particles moving through it by changing their movement.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mode` | **[ForceMode](https://wiki.resonite.com/index.php?title=Type:ForceMode&action=edit&redlink=1 "Type:ForceMode (page does not exist)")** | How to affect Particles in terms of force. |
| `Strength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How strong is the force effect. |
| `GlobalNoiseOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The 4th dimensional offset of the noise. Essentially a seed. |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to scale up or down the noise from it's center. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to shift the noise on its axies. |
| `X_NoiseOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the noise on the X axis. |
| `Y_NoiseOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the noise on the Y axis. |
| `Z_NoiseOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the noise on the Z axis. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:RadialForce](https://wiki.resonite.com/Component:RadialForce "Component:RadialForce")
- [Component:LinearForce](https://wiki.resonite.com/Component:LinearForce "Component:LinearForce")
- [Component:GravityForce](https://wiki.resonite.com/Component:GravityForce "Component:GravityForce")
- [Component:Texture3D Force](https://wiki.resonite.com/Component:Texture3D_Force "Component:Texture3D Force")
- Component:SimplexTurbulentForce
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SimplexTurbulentForce&oldid=96039](https://wiki.resonite.com/index.php?title=Component:SimplexTurbulentForce&oldid=96039)"

Contents