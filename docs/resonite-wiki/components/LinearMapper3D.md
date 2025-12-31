# Component:LinearMapper3D

> Source: https://wiki.resonite.com/Component:LinearMapper3D

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LinearMapper3D&diff=96495) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/13/LinearMapper3DComponent.png/510px-LinearMapper3DComponent.png)](https://wiki.resonite.com/File:LinearMapper3DComponent.png) **Linear Mapper 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Linear Mapper 3D is a component that draws a line from `TargetMin` and `TargetMax` and uses a linear range between the two with `Target` to map `Source` to a range between `SourceMin` and `SourceMax`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The value to map from `SourceMin` to `SourceMax` using `Target`. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The value to map from `TargetMin` to `TargetMax` using `Source`. |
| `SourceMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum of the range of the `Source` value. |
| `SourceMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum of the range of the `Source` value. |
| `TargetMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minimum of the range of the `Target` value. |
| `TargetMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum of the range of the `Target` value. |
| `AllowReverseMapping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow `Target` to map it's value to `Source`'s ranged value when written to. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `Clamp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent `Source` and `Target` from going outside their defined ranges. |

Fields
Collapse

## Usage

## Examples

- [LinearMapper tutorial](https://www.youtube.com/watch?v=B8skjptmLiU) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

- [LinearMapper1D](https://wiki.resonite.com/Component:LinearMapper1D "Component:LinearMapper1D")
- [LinearMapper2D](https://wiki.resonite.com/Component:LinearMapper2D "Component:LinearMapper2D")
- LinearMapper3D
- [LinearMapper4D](https://wiki.resonite.com/Component:LinearMapper4D "Component:LinearMapper4D")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LinearMapper3D&oldid=96495](https://wiki.resonite.com/index.php?title=Component:LinearMapper3D&oldid=96495)"

Contents