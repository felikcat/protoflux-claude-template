# Component:CurrentDateTimeTextDriver

> Source: https://wiki.resonite.com/Component:CurrentDateTimeTextDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8b/CurrentDateTimeTextDriverComponent.png/510px-CurrentDateTimeTextDriverComponent.png)](https://wiki.resonite.com/File:CurrentDateTimeTextDriverComponent.png) **Current Date Time Text Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CurrentDateTimeTextDriver** component takes the current time and formats it using C# DateTime to string using format as an argument.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | What to drive the contents to be the current time formatted. |
| `Pattern` | **[DateTimePattern](https://wiki.resonite.com/index.php?title=Type:DateTimePattern&action=edit&redlink=1 "Type:DateTimePattern (page does not exist)")** | The pattern to use when rendering the date time, EX: 24 vs 12 hr. |
| `UseUTC` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the current time outputted should be UTC time zone. |
| `OverrideFormat` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the outputted current time. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

See the [.NET Standard date and time format strings](https://learn.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings) for DateTimePattern values:

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CurrentDateTimeTextDriver&oldid=98767](https://wiki.resonite.com/index.php?title=Component:CurrentDateTimeTextDriver&oldid=98767)"

Contents