# Component:LocalDateTimeConvertor

> Source: https://wiki.resonite.com/Component:LocalDateTimeConvertor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b4/LocalDateTimeConvertorComponent.png/510px-LocalDateTimeConvertorComponent.png)](https://wiki.resonite.com/File:LocalDateTimeConvertorComponent.png) **Local Date Time Convertor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The LocalDateTimeConvertor converts an inputted time to the user's local timezone.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime") >>** | The source field holding the date time to convert. |
| `LocalDateTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The value of the field targeted by `Source` converted to the local user's datetime. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocalDateTimeConvertor&oldid=94868](https://wiki.resonite.com/index.php?title=Component:LocalDateTimeConvertor&oldid=94868)"

Contents