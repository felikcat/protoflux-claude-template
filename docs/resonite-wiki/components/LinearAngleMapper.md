# Component:LinearAngleMapper

> Source: https://wiki.resonite.com/Component:LinearAngleMapper

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LinearAngleMapper&diff=96497) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/ba/LinearAngleMapperComponent.png/510px-LinearAngleMapperComponent.png)](https://wiki.resonite.com/File:LinearAngleMapperComponent.png) **Linear Angle Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LinearAngleMapper** component is used to map a float range to a rotation range using lerp.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The source value field to get the source mapped value from. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation to drive with the mapped rotation value. |
| `SourceMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value for `Source` for mapping. |
| `SourceMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value for `Source` for mapping. |
| `TargetMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The minumum rotation value when `Source` is at `SourceMin`'s value. |
| `TargetMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum rotation value when `Source` is at `SourceMax`'s value. |
| `AllowReverseMapping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to `Target` map in the reverse direction and get applied to target. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `Clamp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow extrapolation of the lerped data or to keep it within the values specified. |

Fields
Collapse

## Examples

Can be used to make an object spin as a slider is slid. Then can also be used to rotate the object that in turn affects the slider if `AllowReverseMapping` is enabled.

## See Also

- [Component:LinearRotationMapper](https://wiki.resonite.com/Component:LinearRotationMapper "Component:LinearRotationMapper")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LinearAngleMapper&oldid=96497](https://wiki.resonite.com/index.php?title=Component:LinearAngleMapper&oldid=96497)"

Contents