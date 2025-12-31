# Component:LinearForce

> Source: https://wiki.resonite.com/Component:LinearForce

Collapse **Component image**

[File:LinearForceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LinearForceComponent.png "File:LinearForceComponent.png") **Linear Force** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LinearForce** component applies force to all particles within a system towards a direction regardless of particle position.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Force` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction to force particles in. |
| `OverrideForceSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | What Transform space the force direction is in rather than in the particle system's local space. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:RadialForce](https://wiki.resonite.com/Component:RadialForce "Component:RadialForce")
- Component:LinearForce
- [Component:GravityForce](https://wiki.resonite.com/Component:GravityForce "Component:GravityForce")
- [Component:Texture3D Force](https://wiki.resonite.com/Component:Texture3D_Force "Component:Texture3D Force")
- [Component:SimplexTurbulentForce](https://wiki.resonite.com/Component:SimplexTurbulentForce "Component:SimplexTurbulentForce")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LinearForce&oldid=96038](https://wiki.resonite.com/index.php?title=Component:LinearForce&oldid=96038)"

Contents