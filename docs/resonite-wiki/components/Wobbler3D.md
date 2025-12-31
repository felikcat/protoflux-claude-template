# Component:Wobbler3D

> Source: https://wiki.resonite.com/Component:Wobbler3D

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Wobbler3D&diff=92403) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/88/Wobbler3DComponent.png/510px-Wobbler3DComponent.png)](https://wiki.resonite.com/File:Wobbler3DComponent.png) **Wobbler 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Wobbler3D** component can be used to make a value randomly change in a smooth fashion.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to wobble. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The starting point of the wobble. |
| `Speed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | how fast to wobble. |
| `Magnitude` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the amount to wobble from `Offset` |
| `Seed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the value to use as a seed for the randomness. |

Fields
Collapse

## Usage

- [Wobble things with the Wobbler](https://www.youtube.com/watch?v=fJ5-IXKNq1Q) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Wobbler1D](https://wiki.resonite.com/Component:Wobbler1D "Component:Wobbler1D")
- [Component:Wobbler2D](https://wiki.resonite.com/Component:Wobbler2D "Component:Wobbler2D")
- Component:Wobbler3D
- [Component:Wobbler4D](https://wiki.resonite.com/Component:Wobbler4D "Component:Wobbler4D")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Wobbler3D&oldid=92403](https://wiki.resonite.com/index.php?title=Component:Wobbler3D&oldid=92403)"

Contents