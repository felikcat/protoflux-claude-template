# Component:SetAssetReference

> Source: https://wiki.resonite.com/Component:SetAssetReference

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/90/SetAssetReference%601Component.png/510px-SetAssetReference%601Component.png)](https://wiki.resonite.com/File:SetAssetReference%601Component.png) **Set Asset Reference\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Set Asset Reference** component is used to store an [undo](https://wiki.resonite.com/Undo "Undo") step for setting a reference field for assets to another asset.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") <A>** | The field that was changed. |
| `TargetBefore` | **A** | The asset value before the change |
| `TargetAfter` | **A** | The asset value after the change. |
| `_performed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the undo step was done or undone. |
| `_description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of the change that was made and what to for the context menu label text when undoing/redoing. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

See [Undo](https://wiki.resonite.com/Undo "Undo").

## See Also

- [Undo](https://wiki.resonite.com/Undo "Undo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SetAssetReference&oldid=100863](https://wiki.resonite.com/index.php?title=Component:SetAssetReference&oldid=100863)"

Contents