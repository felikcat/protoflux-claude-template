# Component:ColorFromTexture3D

> Source: https://wiki.resonite.com/Component:ColorFromTexture3D

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ee/ColorFromTexture3DComponent.png/510px-ColorFromTexture3DComponent.png)](https://wiki.resonite.com/File:ColorFromTexture3DComponent.png) **Color From Texture 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorFromTexture3D** component makes particles sample their color from the color in their same position within a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D").

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture3D` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The 3D texture to sample from. |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much bias to choose higher axis values. The default is 1 which is no bias. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to add to the chosen point in the 3D texture, which can cut off lower or higher values from ever being chosen. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- Component:ColorFromTexture3D
- [Component:ColorRangeInitializer](https://wiki.resonite.com/Component:ColorRangeInitializer "Component:ColorRangeInitializer")
- [Component:ColorConstantInitializer](https://wiki.resonite.com/Component:ColorConstantInitializer "Component:ColorConstantInitializer")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorFromTexture3D&oldid=113614](https://wiki.resonite.com/index.php?title=Component:ColorFromTexture3D&oldid=113614)"

Contents