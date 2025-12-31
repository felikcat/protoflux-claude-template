# Component:LinearColorMapper

> Source: https://wiki.resonite.com/Component:LinearColorMapper

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LinearColorMapper&diff=96496) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/78/LinearColorMapperComponent.png/510px-LinearColorMapperComponent.png)](https://wiki.resonite.com/File:LinearColorMapperComponent.png) **Linear Color Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LinearColorMapper** allows for mapping a float to a color range, and optionally do so in reverse.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The value to map from `SourceMin` to `SourceMax` using `Target`. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The value to map from `TargetMin` to `TargetMax` using `Source`. |
| `SourceMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum of the range of the `Source` value. |
| `SourceMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum of the range of the `Source` value. |
| `TargetMin` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The minimum of the range of the `Target` value. |
| `TargetMax` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The maximum of the range of the `Target` value. |
| `AllowReverseMapping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow `Target` to map it's value to `Source`'s ranged value when written to. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `Clamp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent `Source` and `Target` from going outside their defined ranges. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LinearColorMapper&oldid=96496](https://wiki.resonite.com/index.php?title=Component:LinearColorMapper&oldid=96496)"

Contents