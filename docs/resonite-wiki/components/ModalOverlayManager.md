# Component:ModalOverlayManager

> Source: https://wiki.resonite.com/Component:ModalOverlayManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ModalOverlayManager&diff=106610) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c0/ModalOverlayManagerComponent.png/510px-ModalOverlayManagerComponent.png)](https://wiki.resonite.com/File:ModalOverlayManagerComponent.png) **ModalOverlayManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ModalOverlayManager** component allows for the creation of [ModalOverlay](https://wiki.resonite.com/Component:ModalOverlay "Component:ModalOverlay") [slots](https://wiki.resonite.com/Slot "Slot"). Using the `Template` field to create Modal Overlays duplicates.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Template` | **[ModalOverlay](https://wiki.resonite.com/Component:ModalOverlay "Component:ModalOverlay")** | The template ModalOverlay slot. |
| `Constructor` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ModalOverlayConstructor](https://wiki.resonite.com/index.php?title=Type:ModalOverlayConstructor&action=edit&redlink=1 "Type:ModalOverlayConstructor (page does not exist)")** | The constructor to make the ModalOverlay. |
| `ModalOverlayRequested` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <ModalOverlayManager>** | The action of the ModalOverlayManager. |
| `ModalOverlayGenerated` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") <ModalOverlayManager, [ModalOverlay](https://wiki.resonite.com/Component:ModalOverlay "Component:ModalOverlay") >** | The action of the ModalOverlayManager. |
| `SpawnRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot hierarchy to spawn this modal overlay on. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ModalOverlayManager&oldid=106610](https://wiki.resonite.com/index.php?title=Component:ModalOverlayManager&oldid=106610)"

Contents