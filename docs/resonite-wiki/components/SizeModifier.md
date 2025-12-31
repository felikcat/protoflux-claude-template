# Component:SizeModifier

> Source: https://wiki.resonite.com/Component:SizeModifier

Collapse **Component image**

[File:SizeModifierComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SizeModifierComponent.png "File:SizeModifierComponent.png") **Size Modifier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SizeModifier** component modifies the size of particles as an extra effect on top of existing size modifiers.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Multiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to multiply the size of all particles. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to add to the size of all particles. |
| `SizeClampMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum size particles can be. |
| `SizeClampMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum size particles can be. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SizeModifier&oldid=96093](https://wiki.resonite.com/index.php?title=Component:SizeModifier&oldid=96093)"

Contents