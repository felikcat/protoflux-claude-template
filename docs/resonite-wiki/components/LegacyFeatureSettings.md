# Component:LegacyFeatureSettings

> Source: https://wiki.resonite.com/Component:LegacyFeatureSettings

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b3/LegacyFeatureSettingsComponent.png/510px-LegacyFeatureSettingsComponent.png)](https://wiki.resonite.com/File:LegacyFeatureSettingsComponent.png) **Legacy Feature Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyFeatureSettings** component is best described on it's page, [Settings](https://wiki.resonite.com/Settings "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseLegacyGripEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Toggles the ability to quick equip tools. |
| `UseLegacyWorldSwitcher` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Toggles the old way of switching between [sessions](https://wiki.resonite.com/Session "Session"). |
| `UseLegacyInventorySessionShortcuts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Toggles the [Legacy Inventory](https://wiki.resonite.com/Legacy_Inventory "Legacy Inventory") window. (Use left grip + dash menu button in VR, or use Ctrl + i in Desktop). |
| `SuppressFeetSimulation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This is to make certain features like posers that hijack feet proxies work, without having to modify them.<br>If you turn this on without using posers or similar features, the animations will NOT look correct. Turn this off after you’re done using posers.<br>_This will likely be removed at some point, we recommend upgrading posers to be compatible with the new system and automatically suppress the simulation when active._ |

Fields
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyFeatureSettings&oldid=99017](https://wiki.resonite.com/index.php?title=Component:LegacyFeatureSettings&oldid=99017)"

Contents