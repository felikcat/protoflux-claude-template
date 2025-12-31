# Component:ConvertibleUshortDriver

> Source: https://wiki.resonite.com/Component:ConvertibleUshortDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/91/ConvertibleUshortDriver%601Component.png/510px-ConvertibleUshortDriver%601Component.png)](https://wiki.resonite.com/File:ConvertibleUshortDriver%601Component.png) **Convertible Ushort Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConvertibleUshortDriver** component is used to convert a value into a Ushort using the value's convert to Ushort method.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value to convert. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Ushort](https://wiki.resonite.com/Type:Ushort "Type:Ushort")** | The field to drive with `Source` converted into a Ushort. |

Fields
Collapse

## Usage

Used to convert values from one type into another via Components rather than [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConvertibleUshortDriver&oldid=96331](https://wiki.resonite.com/index.php?title=Component:ConvertibleUshortDriver&oldid=96331)"

Contents