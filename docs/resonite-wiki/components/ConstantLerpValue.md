# Component:ConstantLerpValue

> Source: https://wiki.resonite.com/Component:ConstantLerpValue

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/ConstantLerpValue%601Component.png/510px-ConstantLerpValue%601Component.png)](https://wiki.resonite.com/File:ConstantLerpValue%601Component.png) **Constant Lerp Value** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConstantLerpValue** component will make the `Value` reach `TargetValue`, making `Speed` progress per second. it can also be known as a linear lerp.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetValue` | **T** | The value to stop at. |
| `Speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to change `Value` by per second to reach `TargetValue` |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to `Value` will be written to `TargetValue`. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `Value` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The value to constantly progress towards `TargetValue` |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConstantLerpValue&oldid=105899](https://wiki.resonite.com/index.php?title=Component:ConstantLerpValue&oldid=105899)"

Contents