# Component:Panner3D

> Source: https://wiki.resonite.com/Component:Panner3D

<translate>

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/Panner3DComponent.png/510px-Panner3DComponent.png)](https://wiki.resonite.com/File:Panner3DComponent.png) **Panner 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Makes a value change constantly between a range over time.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to change over time. |
| `_offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to add to the output value after all other calculations. |
| `_preOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | At what point to start at after item start. |
| `_speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to progress the value |
| `_repeat` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | At what value to repeat |
| `PingPong` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to bounce back and forth between zero and `_repeat`. |

Fields
Collapse

## Usage

## Examples

- [Panner tutorial](https://www.youtube.com/watch?v=S0dF4bdtT6Q) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

</translate>

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Panner3D&oldid=98464](https://wiki.resonite.com/index.php?title=Component:Panner3D&oldid=98464)"

Contents