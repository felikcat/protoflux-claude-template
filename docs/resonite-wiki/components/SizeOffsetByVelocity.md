# Component:SizeOffsetByVelocity

> Source: https://wiki.resonite.com/Component:SizeOffsetByVelocity

Collapse **Component image**

[File:SizeOffsetByVelocityComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SizeOffsetByVelocityComponent.png "File:SizeOffsetByVelocityComponent.png") **Size Offset By Velocity** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SizeOffsetByVelocity** component changes the size of particles in a particle system based on their velocity.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VelocityMultiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much velocity should multiply the size of the particle. |
| `OffsetClampMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum value for the clamping of the offset. |
| `OffsetClampMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum value for the clamping of the offset. |
| `ResultClampMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum value for the clamping of the result. |
| `ResultClampMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum value for the clamping of the result. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SizeOffsetByVelocity&oldid=96092](https://wiki.resonite.com/index.php?title=Component:SizeOffsetByVelocity&oldid=96092)"

Contents