# Component:PositionSimulatorModule

> Source: https://wiki.resonite.com/Component:PositionSimulatorModule

Collapse **Component image**

[File:PositionSimulatorModuleComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=PositionSimulatorModuleComponent.png "File:PositionSimulatorModuleComponent.png") **Position Simulator Module** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PositionSimulatorModule** component is the most essential particle simulator module. Without it, particles will not move, and won't have velocity.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Collisions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether particles should have collisions. |
| `CollisionLifetimeLossRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much lifetime percentage from 0<->1 should particles loose when hitting a surface? |
| `CollisionBounceRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much velocity should particles retain as a percentage from 0<->1 when bouncing off of a surface? |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- Component:PositionSimulatorModule
- [Component:RotationSimulatorModule](https://wiki.resonite.com/Component:RotationSimulatorModule "Component:RotationSimulatorModule")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PositionSimulatorModule&oldid=96044](https://wiki.resonite.com/index.php?title=Component:PositionSimulatorModule&oldid=96044)"

Contents