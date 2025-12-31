# Component:ConvertibleDecimalDriver

> Source: https://wiki.resonite.com/Component:ConvertibleDecimalDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/ConvertibleDecimalDriver%601Component.png/510px-ConvertibleDecimalDriver%601Component.png)](https://wiki.resonite.com/File:ConvertibleDecimalDriver%601Component.png) **Convertible Decimal Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConvertibleDecimalDriver** component is used to convert a value into a Decimal using the value's convert to Decimal method.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value to convert. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Decimal](https://wiki.resonite.com/Type:Decimal "Type:Decimal")** | The field to drive with `Source` converted into a Decimal. |

Fields
Collapse

## Usage

Used to convert values from one type into another via Components rather than [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConvertibleDecimalDriver&oldid=96341](https://wiki.resonite.com/index.php?title=Component:ConvertibleDecimalDriver&oldid=96341)"

Contents