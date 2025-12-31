# Component:ValueTextFormatDriver

> Source: https://wiki.resonite.com/Component:ValueTextFormatDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ValueTextFormatDriver&diff=113352) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/97/ValueTextFormatDriver%601Component.png/510px-ValueTextFormatDriver%601Component.png)](https://wiki.resonite.com/File:ValueTextFormatDriver%601Component.png) **Value Text Format Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

**ValueTextFormatDriver** applies the value of a single source field to a [text format string](https://docs.microsoft.com/en-us/dotnet/api/system.string.format?view=net-5.0#get-started-with-the-stringformat-method) and drives the target string field. The source field is element 0 in the format string. Elements are defined by putting {} brackets around a number. Although the image shown and the field list below have the source field being a float, this component is generic, so any field type (that can be converted to a string) can be used.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The source field for the value. |
| `Format` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string format with "{0}" in it somewhere |
| `Text` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The target field. |

Fields
Collapse

## Usage

Attach to a slot and provide a format string and source value in order to drive a string field (possibly text) with the formatted number.

## Examples

[![](https://wiki.resonite.com/images/thumb/7/79/ValueTextFormatDriverExample1.png/300px-ValueTextFormatDriverExample1.png)](https://wiki.resonite.com/File:ValueTextFormatDriverExample1.png) Screenshot of a quick example using ValueTextFormatDriver

Can be used to drive the descriptions on [UIX](https://wiki.resonite.com/UIX "UIX"), context menus, or visuals without involving flux.

## See Also

- [StringConcatenationDriver](https://wiki.resonite.com/Component:StringConcatenationDriver "Component:StringConcatenationDriver") for combining the output with multiple other bits of text for a more robust final product.
- [MultiValueTextFormatDriver](https://wiki.resonite.com/Component:MultiValueTextFormatDriver "Component:MultiValueTextFormatDriver") for more than one source.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueTextFormatDriver&oldid=113352](https://wiki.resonite.com/index.php?title=Component:ValueTextFormatDriver&oldid=113352)"

Contents