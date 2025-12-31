# Component:AppVersionDriver

> Source: https://wiki.resonite.com/Component:AppVersionDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fa/AppVersionDriverComponent.png/510px-AppVersionDriverComponent.png)](https://wiki.resonite.com/File:AppVersionDriverComponent.png) **App Version Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

App version driver is a component that drives the content of the string field provided to `Text` to Resonite's version.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Text` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Drives the provided text field's content to Resonite's version. The text is formatted starting with "Beta", "Alpha", or "Release", followed by the game's compile date. The date is formatted `year.day.month.minuteOfDay`. Minute of day is the minutes since midnight. The time is in UTC. |

Fields
Collapse

## Behavior

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AppVersionDriver&oldid=88748](https://wiki.resonite.com/index.php?title=Component:AppVersionDriver&oldid=88748)"

Contents