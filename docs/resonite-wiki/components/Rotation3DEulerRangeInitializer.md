# Component:Rotation3DEulerRangeInitializer

> Source: https://wiki.resonite.com/Component:Rotation3DEulerRangeInitializer

Collapse **Component image**

[File:Rotation3DEulerRangeInitializerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Rotation3DEulerRangeInitializerComponent.png "File:Rotation3DEulerRangeInitializerComponent.png") **Rotation 3D Euler Range Initializer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Rotation3DEulerRangeInitializer** component makes particles have a random rotation between a pair of Euler angles.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinValue` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum euler angle rotation a particle can have. |
| `MaxValue` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum euler angle rotation a particle can have. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:RotationRangeInitializer](https://wiki.resonite.com/Component:RotationRangeInitializer "Component:RotationRangeInitializer")
- [Component:RotationConstantInitializer](https://wiki.resonite.com/Component:RotationConstantInitializer "Component:RotationConstantInitializer")
- Component:Rotation3DEulerRangeInitializer
- [Component:Rotation3DConstantInitializer](https://wiki.resonite.com/Component:Rotation3DConstantInitializer "Component:Rotation3DConstantInitializer")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Rotation3DEulerRangeInitializer&oldid=96074](https://wiki.resonite.com/index.php?title=Component:Rotation3DEulerRangeInitializer&oldid=96074)"

Contents