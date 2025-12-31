# Component:ConvertibleUlongDriver

> Source: https://wiki.resonite.com/Component:ConvertibleUlongDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b3/ConvertibleUlongDriver%601Component.png/510px-ConvertibleUlongDriver%601Component.png)](https://wiki.resonite.com/File:ConvertibleUlongDriver%601Component.png) **Convertible Ulong Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConvertibleUlongDriver** component is used to convert a value into a Ulong using the value's convert to Ulong method.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value to convert. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Ulong](https://wiki.resonite.com/Type:Ulong "Type:Ulong")** | The field to drive with `Source` converted into a Ulong. |

Fields
Collapse

## Usage

Used to convert values from one type into another via Components rather than [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConvertibleUlongDriver&oldid=96332](https://wiki.resonite.com/index.php?title=Component:ConvertibleUlongDriver&oldid=96332)"

Contents