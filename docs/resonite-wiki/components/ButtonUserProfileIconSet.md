# Component:ButtonUserProfileIconSet

> Source: https://wiki.resonite.com/Component:ButtonUserProfileIconSet

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonUserProfileIconSet&diff=90377) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/06/ButtonUserProfileIconSet.png/510px-ButtonUserProfileIconSet.png)](https://wiki.resonite.com/File:ButtonUserProfileIconSet.png) **Button User Profile Icon Set** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonUserProfileIconSet** component only works in [Userspace](https://wiki.resonite.com/Userspace "Userspace"). This is the component that handles the setting of a user profile icon in the game.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsUpdating` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the component is sending to the cloud your new icon [url](https://wiki.resonite.com/Type:Uri "Type:Uri") and/or asset. |

Fields
Collapse

## Usage

Put this beside a [button](https://wiki.resonite.com/Type:IButton "Type:IButton") component on an [slot](https://wiki.resonite.com/Slot "Slot") or [facet](https://wiki.resonite.com/Facets "Facets") and press the button to set your profile icon via the button.

## Examples

The user profile default facet that comes with your dash upon making a new account.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonUserProfileIconSet&oldid=90377](https://wiki.resonite.com/index.php?title=Component:ButtonUserProfileIconSet&oldid=90377)"

Contents