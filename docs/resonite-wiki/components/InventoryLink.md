# Component:InventoryLink

> Source: https://wiki.resonite.com/Component:InventoryLink

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:InventoryLink&diff=98934) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ac/InventoryLinkComponent.png/510px-InventoryLinkComponent.png)](https://wiki.resonite.com/File:InventoryLinkComponent.png) **Inventory Link** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component overrides the saving behavior of an item being saved to act as an inventory folder. The component will be overridden by another component if it is under another slot on an item with a different export behavior. (Ex: A [Texture Exportable Component](https://wiki.resonite.com/Component:TextureExportable "Component:TextureExportable"))

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the folder this component is linking to. This will change the display name of the folder when saved, but if shared by the same user again from their inventory, this will become what the cloud says the folder's name is and not the custom name it was when saved. |
| `Target` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The folder URI link on the cloud that this component represents. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCopyLink:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to copy the link for this component via their context menu. |

Triggers
Collapse

## Usage

Attach to a slot and give the component a `TargetName` and a URI that links to a folder on the cloud for the `Target` saving an item with this component on it will make the item act like a folder link.

## Examples

Is the core component that drives the saving behavior of shared folder links within the world. (Those blue rectangle styled folders with a name on them)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InventoryLink&oldid=98934](https://wiki.resonite.com/index.php?title=Component:InventoryLink&oldid=98934)"

Contents