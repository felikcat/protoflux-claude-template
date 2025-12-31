# Component:UserInterfaceEditModeSync

> Source: https://wiki.resonite.com/Component:UserInterfaceEditModeSync

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/87/UserInterfaceEditModeSyncComponent.png/510px-UserInterfaceEditModeSyncComponent.png)](https://wiki.resonite.com/File:UserInterfaceEditModeSyncComponent.png) **User Interface Edit Mode Sync** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserInterfaceEditModeSync** component allows a world to tell if a user is currently in edit mode.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to check edit mode for. |
| `EditModeActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `TargetUser` is in edit mode. |

Fields
Collapse

## Usage

Attach to a slot and either drive or set the values of the contained `TargetUser` to get an edit mode status.

## Examples

Can be used to make world or item elements that should only be used in edit mode (basically super developer).

## See Also

- [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") what is edit mode?

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserInterfaceEditModeSync&oldid=95826](https://wiki.resonite.com/index.php?title=Component:UserInterfaceEditModeSync&oldid=95826)"

Contents