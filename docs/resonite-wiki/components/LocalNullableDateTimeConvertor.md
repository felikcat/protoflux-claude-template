# Component:LocalNullableDateTimeConvertor

> Source: https://wiki.resonite.com/Component:LocalNullableDateTimeConvertor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d5/LocalNullableDateTimeConvertorComponent.png/510px-LocalNullableDateTimeConvertorComponent.png)](https://wiki.resonite.com/File:LocalNullableDateTimeConvertorComponent.png) **Local Nullable Date Time Convertor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NullableLocalDateTimeConvertor** converts a nullable inputted time to the user's local timezone.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >>>** | The source field holding the date time to convert. |
| `LocalDateTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >** | The value of the field targeted by `Source` converted to the local user's datetime. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocalNullableDateTimeConvertor&oldid=94867](https://wiki.resonite.com/index.php?title=Component:LocalNullableDateTimeConvertor&oldid=94867)"

Contents