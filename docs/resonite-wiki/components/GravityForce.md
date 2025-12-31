# Component:GravityForce

> Source: https://wiki.resonite.com/Component:GravityForce

Collapse **Component image**

[File:GravityForceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GravityForceComponent.png "File:GravityForceComponent.png") **Gravity Force** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GravityForce** component acts as a global force for particles that makes them fall either up or down along the Up axis.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Gravity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The force to apply. Negative values are down and positive values are up. |
| `OverrideForceSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to calculate gravity force in. Is converted into the particle system's space. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Can be used to simulate gravity on particles In a particle system, or fire/smoke for rising particles.

## See Also

- [Component:RadialForce](https://wiki.resonite.com/Component:RadialForce "Component:RadialForce")
- [Component:LinearForce](https://wiki.resonite.com/Component:LinearForce "Component:LinearForce")
- Component:GravityForce
- [Component:Texture3D Force](https://wiki.resonite.com/Component:Texture3D_Force "Component:Texture3D Force")
- [Component:SimplexTurbulentForce](https://wiki.resonite.com/Component:SimplexTurbulentForce "Component:SimplexTurbulentForce")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GravityForce&oldid=96042](https://wiki.resonite.com/index.php?title=Component:GravityForce&oldid=96042)"

Contents