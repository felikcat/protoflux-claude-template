# Component:OnlineStatusSettings

> Source: https://wiki.resonite.com/Component:OnlineStatusSettings

Collapse **Component image**

[File:OnlineStatusSettingsComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=OnlineStatusSettingsComponent.png "File:OnlineStatusSettingsComponent.png") **Online Status Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OnlineStatusSettings** component is used to define how online status for the user should be handled.

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DefaultStatus` | **[OnlineStatus](https://wiki.resonite.com/index.php?title=Type:OnlineStatus&action=edit&redlink=1 "Type:OnlineStatus (page does not exist)")** | The default status for the user when they log in. |
| `RememberMode` | **[OnlineStatusSettings.StatusRememberMode](https://wiki.resonite.com/Component:OnlineStatusSettings#StatusRememberMode)** | Whether the status the user had when they were last on should be remembered. |
| `RememberTimespan` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | How long to remember the last status from the previous login before setting back to default again. |
| `InvisibleRememberMode` | **[OnlineStatusSettings.StatusRememberMode](https://wiki.resonite.com/Component:OnlineStatusSettings#StatusRememberMode)** | How to remember the previous status from the last login. |
| `InvisibleRememberTimespan` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | How long to remember a status if it's set to invisible. |
| `AutoAwayTimespan` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | How long to wait when the user is AFK before enabling Away. |
| `EnableDefaultStatus` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enable the default status behavior. |
| `ShowRememberTimespan` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the remember timespan control UI. |
| `ShowInvisibleRememberTimespan` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the remember invisible timespan control UI. |

Fields
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

See [Settings](https://wiki.resonite.com/Settings "Settings").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OnlineStatusSettings&oldid=105351](https://wiki.resonite.com/index.php?title=Component:OnlineStatusSettings&oldid=105351)"

Contents