# Component:Rotation3DConstantInitializer

> Source: https://wiki.resonite.com/Component:Rotation3DConstantInitializer

Collapse **Component image**

[File:Rotation3DConstantInitializerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Rotation3DConstantInitializerComponent.png "File:Rotation3DConstantInitializerComponent.png") **Rotation 3D Constant Initializer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Rotation3DConstantInitializer** component gives all particles a starting rotation of `Value` upon creation.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The starting rotation all particles should have. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:RotationRangeInitializer](https://wiki.resonite.com/Component:RotationRangeInitializer "Component:RotationRangeInitializer")
- [Component:RotationConstantInitializer](https://wiki.resonite.com/Component:RotationConstantInitializer "Component:RotationConstantInitializer")
- [Component:Rotation3DEulerRangeInitializer](https://wiki.resonite.com/Component:Rotation3DEulerRangeInitializer "Component:Rotation3DEulerRangeInitializer")
- Component:Rotation3DConstantInitializer
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Rotation3DConstantInitializer&oldid=96075](https://wiki.resonite.com/index.php?title=Component:Rotation3DConstantInitializer&oldid=96075)"

Contents