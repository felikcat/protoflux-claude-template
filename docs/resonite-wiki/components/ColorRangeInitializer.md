# Component:ColorRangeInitializer

> Source: https://wiki.resonite.com/Component:ColorRangeInitializer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/35/ColorRangeInitializerComponent.png/510px-ColorRangeInitializerComponent.png)](https://wiki.resonite.com/File:ColorRangeInitializerComponent.png) **Color Range Initializer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorRangeInitializer** component gives particles a random color lerped between a min and Max color when they are born.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinValue` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The minimum color a Particle could have when born. |
| `MaxValue` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The maximum color a Particle could have when born. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ColorFromTexture3D](https://wiki.resonite.com/Component:ColorFromTexture3D "Component:ColorFromTexture3D")
- Component:ColorRangeInitializer
- [Component:ColorConstantInitializer](https://wiki.resonite.com/Component:ColorConstantInitializer "Component:ColorConstantInitializer")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorRangeInitializer&oldid=96026](https://wiki.resonite.com/index.php?title=Component:ColorRangeInitializer&oldid=96026)"

Contents