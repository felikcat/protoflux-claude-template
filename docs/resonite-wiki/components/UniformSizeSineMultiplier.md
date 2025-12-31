# Component:UniformSizeSineMultiplier

> Source: https://wiki.resonite.com/Component:UniformSizeSineMultiplier

Collapse **Component image**

[File:UniformSizeSineMultiplierComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=UniformSizeSineMultiplierComponent.png "File:UniformSizeSineMultiplierComponent.png") **Uniform Size Sine Multiplier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UniformSizeSineMultiplier** component makes particles start their size multipled by the current point in a constantly changing Sine wave.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed of the Sine Wave change. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The initial offset of the Sine Wave. |
| `MinMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum Sine Wave value that can be outputted and multipled with the particle's starting size. |
| `MaxMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum Sine Wave value that can be outputted and multipled with the particle's starting size. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:UniformSizeConstantInitializer](https://wiki.resonite.com/Component:UniformSizeConstantInitializer "Component:UniformSizeConstantInitializer") \\* [Component:UniformSizeOverLifetimeStartEnd](https://wiki.resonite.com/Component:UniformSizeOverLifetimeStartEnd "Component:UniformSizeOverLifetimeStartEnd")
- [Component:UniformSizeRangeInitializer](https://wiki.resonite.com/Component:UniformSizeRangeInitializer "Component:UniformSizeRangeInitializer")
- Component:UniformSizeSineMultiplier
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UniformSizeSineMultiplier&oldid=96077](https://wiki.resonite.com/index.php?title=Component:UniformSizeSineMultiplier&oldid=96077)"

Contents