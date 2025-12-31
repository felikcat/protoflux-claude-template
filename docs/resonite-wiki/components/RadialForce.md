# Component:RadialForce

> Source: https://wiki.resonite.com/Component:RadialForce

Collapse **Component image**

[File:RadialForceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=RadialForceComponent.png "File:RadialForceComponent.png") **Radial Force** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RadialForce** component makes particles attracted or repelled from a point in 3D space when they get closer or further away. The gradient for the force does not cut off at `MinDistance` and/or `MaxDistance`. instead the gradient continues into infinity at the value it was when it hits these values. The `Force` determines the distance truely if `MinDistance` is at 0 and `MaxDistance` is at infinity.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Force` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much force this component exerts on particles in a system. |
| `Mode` | **[RadialForceMode](https://wiki.resonite.com/index.php?title=Type:RadialForceMode&action=edit&redlink=1 "Type:RadialForceMode (page does not exist)")** | How to determine how the force is calculated. |
| `MinDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum distance for the force gradient, aka force gradient start point, the gradient does not stop here. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum distance for the force gradient, aka force gradient start point, the gradient does not stop here. |
| `MinForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much force should be applied at `MinDistance` modified by `Force`. |
| `MaxForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much force should be applied at `MaxDistance` modified by `Force`. |
| `OverrideForceSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to calculate this component's values in. The values get converted to the particle system's space. |
| `Center` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The center point of the force point. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Can be used for orbits, moving particles via a user's hands, and for many other effects.

## See Also

- Component:RadialForce
- [Component:LinearForce](https://wiki.resonite.com/Component:LinearForce "Component:LinearForce")
- [Component:GravityForce](https://wiki.resonite.com/Component:GravityForce "Component:GravityForce")
- [Component:Texture3D Force](https://wiki.resonite.com/Component:Texture3D_Force "Component:Texture3D Force")
- [Component:SimplexTurbulentForce](https://wiki.resonite.com/Component:SimplexTurbulentForce "Component:SimplexTurbulentForce")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadialForce&oldid=106529](https://wiki.resonite.com/index.php?title=Component:RadialForce&oldid=106529)"

Contents