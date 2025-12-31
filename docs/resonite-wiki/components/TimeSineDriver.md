# Component:TimeSineDriver

> Source: https://wiki.resonite.com/Component:TimeSineDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ed/TimeSineDriverComponent.png/510px-TimeSineDriverComponent.png)](https://wiki.resonite.com/File:TimeSineDriverComponent.png) **Time Sine Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TimeSineDriver** component outputs a value over time that matches a Sine Wave of the provided values.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with a constantly changing Sine wave. |
| `Speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The frequency/speed of the Sine Wave waves. |
| `Min` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value to drive `Target` to. |
| `Max` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value to drive `Target` to. |

Fields
Collapse

## Usage

Attach to a slot and provide a `Target` for it to start working.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TimeSineDriver&oldid=95740](https://wiki.resonite.com/index.php?title=Component:TimeSineDriver&oldid=95740)"

Contents