# Component:SizeSineMultiplier

> Source: https://wiki.resonite.com/Component:SizeSineMultiplier

Collapse **Component image**

[File:SizeSineMultiplierComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SizeSineMultiplierComponent.png "File:SizeSineMultiplierComponent.png") **Size Sine Multiplier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SizeSineMultiplier** component makes particles multiply their size on start with a value sampled from a Sine Wave based on the time they were emitted in a particle system.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Speed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The speed that the Sine Wave changes. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The initial offset of the Sine Wave function. |
| `MinMultiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum value outputted by the sinewave function. |
| `MaxMultiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum value outputted by the sinewave function. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SizeSineMultiplier&oldid=96089](https://wiki.resonite.com/index.php?title=Component:SizeSineMultiplier&oldid=96089)"

Contents