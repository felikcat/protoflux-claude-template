# Component:NullableSourceDriver

> Source: https://wiki.resonite.com/Component:NullableSourceDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/58/NullableSourceDriver%601Component.png/510px-NullableSourceDriver%601Component.png)](https://wiki.resonite.com/File:NullableSourceDriver%601Component.png) **Nullable Source Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NullableSourceDriver** component allows for getting info from a `Source` nullable and driving a set of split fields with content from the nullable. Changes to driven fields by this component can also be reverse written back to `Source`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") <T>>>** | The field to get nullable data from. |
| `Value` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with the value for `Source` if it has a value, or instead drive with `DefaultValue`. |
| `HasValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether `Source` has a value. |
| `DefaultValue` | **T** | The default value if `Source` doesn't have a value. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether writes to the fields driven by this component will update the value of `Source`. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `UpdateDefaultValue` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the default value gets updated when using write back and `Source` has no value. |

Fields
Collapse

## Usage

Can be used to extract data from nullables or write to them using a component only solution.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Nullable Fields](https://wiki.resonite.com/Type:Nullable "Type:Nullable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NullableSourceDriver&oldid=96509](https://wiki.resonite.com/index.php?title=Component:NullableSourceDriver&oldid=96509)"

Contents