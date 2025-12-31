# Component:AppVersion

> Source: https://wiki.resonite.com/Component:AppVersion

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ed/AppVersionComponent.png/510px-AppVersionComponent.png)](https://wiki.resonite.com/File:AppVersionComponent.png) **App Version** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

App version is a component that updates it's fields with the live information of Resonite's version.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VersionNumber` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The version number of Resonite. usually formatted year.month.day.minute. The minute part of the version is the minute from midnight UTC the version was compiled. |
| `VersionName` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the version of Resonite. Usually this is "Beta", "Alpha" or "Release" followed by `VersionNumber` |
| `FullVersionString` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Usually the same as `VersionNumber` |
| `BuildYear` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The year Resonite was compiled. |
| `BuildMonth` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The month Resonite was compiled. |
| `BuildDay` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The day Resonite was compiled. |
| `BuildTimeOfDay` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of minutes since midnight UTC. |

Fields
Collapse

## Behavior

The fields are "Pseudo Driven" or constantly being written to. Attempting to change a field makes it instantly change back and not send an update event.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AppVersion&oldid=98660](https://wiki.resonite.com/index.php?title=Component:AppVersion&oldid=98660)"

Contents