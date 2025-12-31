# Component:VelocityDrag

> Source: https://wiki.resonite.com/Component:VelocityDrag

Collapse **Component image**

[File:VelocityDragComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=VelocityDragComponent.png "File:VelocityDragComponent.png") **Velocity Drag** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VelocityDrag** component makes particles in a particle system slow down towards 0 Velocity when not acted upon as if moving through a substance.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Drag` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to slow down particles to 0 velocity. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Particles moving through water like a rock falling through water and affected by gravity with a [Component:GravityForce](https://wiki.resonite.com/Component:GravityForce "Component:GravityForce").

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VelocityDrag&oldid=96070](https://wiki.resonite.com/index.php?title=Component:VelocityDrag&oldid=96070)"

Contents