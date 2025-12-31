# Component:MultiValueTextFormatDriver

> Source: https://wiki.resonite.com/Component:MultiValueTextFormatDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MultiValueTextFormatDriver&diff=106264) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/MultiValueTextFormatDriverComponent.png/510px-MultiValueTextFormatDriverComponent.png)](https://wiki.resonite.com/File:MultiValueTextFormatDriverComponent.png) **Multi Value Text Format Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueTextFormatDriver** applies the value of a multiple values to a [text format string](https://docs.microsoft.com/en-us/dotnet/api/system.string.format?view=net-5.0#get-started-with-the-stringformat-method) and drives the target string field. Elements are defined by putting {} brackets around a number to specify an element in `Sources`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Sources` | _direct_ **[SyncRelayList\`1](https://wiki.resonite.com/index.php?title=Type:SyncRelayList%601&action=edit&redlink=1 "Type:SyncRelayList`1 (page does not exist)") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | A list of source fields. |
| `Format` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The format string, which has a list of "{X}" where "X" is a number that refers to an item number in `Sources`. The entire "{X}" gets replaced by a source with that number. |
| `Text` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The target field. |

Fields
Collapse

## Usage

## Examples

## See Also

- [ValueTextFormatDriver](https://wiki.resonite.com/ValueTextFormatDriver_(Component) "ValueTextFormatDriver (Component)") <T> when there is a single source.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiValueTextFormatDriver&oldid=106264](https://wiki.resonite.com/index.php?title=Component:MultiValueTextFormatDriver&oldid=106264)"

Contents