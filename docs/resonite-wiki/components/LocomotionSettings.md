# Component:LocomotionSettings

> Source: https://wiki.resonite.com/Component:LocomotionSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/68/LocomotionSettingsComponent.png/510px-LocomotionSettingsComponent.png)](https://wiki.resonite.com/File:LocomotionSettingsComponent.png) **Locomotion Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocomotionSettings** component is better described on the [settings](https://wiki.resonite.com/Settings "Settings") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocomotionPreferences` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[PriorityEntry\`1](https://wiki.resonite.com/index.php?title=Type:PriorityEntry%601&action=edit&redlink=1 "Type:PriorityEntry`1 (page does not exist)") < [LocomotionArchetype](https://wiki.resonite.com/Type:LocomotionArchetype "Type:LocomotionArchetype") >** | A list of locomotion entries that the user prefers when entering a world. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `GetEntry:SubsettingGetter` | **[SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter")** | X | Used to get an entry in the locomotion preference values. |

Triggers
Collapse

## Usage

see [settings](https://wiki.resonite.com/Settings "Settings").

## Examples

see [settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionSettings&oldid=99157](https://wiki.resonite.com/index.php?title=Component:LocomotionSettings&oldid=99157)"

Contents