# Component:SettingsDataFeed

> Source: https://wiki.resonite.com/Component:SettingsDataFeed

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/SettingsDataFeedComponent.png/510px-SettingsDataFeedComponent.png)](https://wiki.resonite.com/File:SettingsDataFeedComponent.png) **Settings Data Feed** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SettingsDataFeed** component is a [data feed](https://wiki.resonite.com/Data_Feed "Data Feed") that generates a list of [settings](https://wiki.resonite.com/Settings "Settings") and their categories.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Using this outside of [userspace](https://wiki.resonite.com/Userspace "Userspace") and interacting with it can crash the session!


## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `PathSegmentName:PathSegmentConverter` | **[PathSegmentConverter](https://wiki.resonite.com/index.php?title=Type:PathSegmentConverter&action=edit&redlink=1 "Type:PathSegmentConverter (page does not exist)")** | X | Gets the locale string of a path using a depth and a name. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used for the settings facet used in the settings tab of the [dash menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingsDataFeed&oldid=99739](https://wiki.resonite.com/index.php?title=Component:SettingsDataFeed&oldid=99739)"

Contents