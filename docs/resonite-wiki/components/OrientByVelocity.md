# Component:OrientByVelocity

> Source: https://wiki.resonite.com/Component:OrientByVelocity

Collapse **Component image**

[File:OrientByVelocityComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=OrientByVelocityComponent.png "File:OrientByVelocityComponent.png") **Orient By Velocity** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OrientByVelocity** component makes particles orient the `Up` axis of the particle in the direction they are moving.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Up` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | What axis of the particle to orient in the direction the particle is moving. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OrientByVelocity&oldid=96036](https://wiki.resonite.com/index.php?title=Component:OrientByVelocity&oldid=96036)"

Contents