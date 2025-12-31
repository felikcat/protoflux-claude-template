# Component:Wiggler

> Source: https://wiki.resonite.com/Component:Wiggler

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Wiggler&diff=92397) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/93/WigglerComponent.png/510px-WigglerComponent.png)](https://wiki.resonite.com/File:WigglerComponent.png) **Wiggler** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Wiggler** component is used to make a [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") rotate randomly. Usually used on a slot's rotation.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to wiggle. |
| `_offset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The base value to "add" to when rotating. |
| `_speed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How fast to wiggle on each axis. |
| `_magnitude` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to wiggle on each axis |
| `_seed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the seed for the randomness of the wiggle. |

Fields
Collapse

## Usage

Used in tails, flags, antennas, and much more random wobbly rotating things.

## Examples

- [Wiggle things with Wiggler](https://www.youtube.com/watch?v=q1dALfAXslo) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Wiggler&oldid=92397](https://wiki.resonite.com/index.php?title=Component:Wiggler&oldid=92397)"

Contents