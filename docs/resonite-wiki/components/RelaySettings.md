# Component:RelaySettings

> Source: https://wiki.resonite.com/Component:RelaySettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1f/RelaySettingsComponent.png/510px-RelaySettingsComponent.png)](https://wiki.resonite.com/File:RelaySettingsComponent.png) **Relay Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

For better info, see [Settings](https://wiki.resonite.com/Settings "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AlwaysUseRelay` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Relays are typically used as a fallback when a direct connection to the host cannot be established. By enabling this option, you will force the connection to always happen through a relay. This can be useful in cases of connection issues to particular hosts. It is NOT recommended to have this option permanently on. |
| `UseClosestAvailableRelay` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When this option is enabled, the closest available relay will be automatically selected. If you want to connect through a specific relay (e.g. in case of long distance connections to avoid packet queuing) you can disable this option and configure the preferred relays below. |
| `RelayPriorities` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[RelayPriorityEntry](https://wiki.resonite.com/index.php?title=Type:RelayPriorityEntry&action=edit&redlink=1 "Type:RelayPriorityEntry (page does not exist)")** | A list of relays to use in order when trying to connect to a host. |
| `RelayPrioritiesEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use the relay priorities list. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `GetEntry:SubsettingGetter` | **[SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter")** | X | Can be used to retrieve an entry from the list of `RelayPriorities`. |

Triggers
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RelaySettings&oldid=106539](https://wiki.resonite.com/index.php?title=Component:RelaySettings&oldid=106539)"

Contents