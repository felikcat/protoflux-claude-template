# Component:RotationRangeInitializer

> Source: https://wiki.resonite.com/Component:RotationRangeInitializer

Collapse **Component image**

[File:RotationRangeInitializerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=RotationRangeInitializerComponent.png "File:RotationRangeInitializerComponent.png") **Rotation Range Initializer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RotationRangeInitializer** component gives particles a random starting rotation within a range along it's orientation axis.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum Rotation that a Particle will start with along it's orientation axis. |
| `MaxValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum rotation that a Particle will start with along it's orientation axis. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- Component:RotationRangeInitializer
- [Component:RotationConstantInitializer](https://wiki.resonite.com/Component:RotationConstantInitializer "Component:RotationConstantInitializer")
- [Component:Rotation3DEulerRangeInitializer](https://wiki.resonite.com/Component:Rotation3DEulerRangeInitializer "Component:Rotation3DEulerRangeInitializer")
- [Component:Rotation3DConstantInitializer](https://wiki.resonite.com/Component:Rotation3DConstantInitializer "Component:Rotation3DConstantInitializer")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RotationRangeInitializer&oldid=96072](https://wiki.resonite.com/index.php?title=Component:RotationRangeInitializer&oldid=96072)"

Contents