# Component:Texture3D Force

> Source: https://wiki.resonite.com/Component:Texture3D_Force

Collapse **Component image**

[File:Texture3D ForceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Texture3D_ForceComponent.png "File:Texture3D ForceComponent.png") **Texture 3D Force** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Texture3DForce** component makes a 3 dimensional field that affects the movement of particles in a particle system based on the colors of a [3D texture](https://wiki.resonite.com/Texture3D "Texture3D"). The colors map from RGB->XYZ in that order. The XYZ mapped value is used to affect the movement of particles.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture3D` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The 3D texture to act as the force volume and to sample colors from in 3D. |
| `Mode` | **[ForceMode](https://wiki.resonite.com/index.php?title=Type:ForceMode&action=edit&redlink=1 "Type:ForceMode (page does not exist)")** | How to affect Particles with the force this component exerts on them. |
| `Strength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength of this component's forvce. |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to scale the 3D texture in physical space along it's axies. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to shift the 3D texture in physical space on it's axies. |
| `ColorBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The bias of colors being sampled from the 3D texture that are being mapped into XYZ values. |
| `ColorScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale the color of pixels in the 3D texture, to change how the force works. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

This allows particles to be able to take custom paths through a volume, collect in wavy shapes, or curve the path of particles going through it.

## See Also

- [Component:RadialForce](https://wiki.resonite.com/Component:RadialForce "Component:RadialForce")
- [Component:LinearForce](https://wiki.resonite.com/Component:LinearForce "Component:LinearForce")
- [Component:GravityForce](https://wiki.resonite.com/Component:GravityForce "Component:GravityForce")
- Component:Texture3D Force
- [Component:SimplexTurbulentForce](https://wiki.resonite.com/Component:SimplexTurbulentForce "Component:SimplexTurbulentForce")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Texture3D\_Force&oldid=113613](https://wiki.resonite.com/index.php?title=Component:Texture3D_Force&oldid=113613)"

Contents