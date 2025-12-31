# Component:AssetReceiver

> Source: https://wiki.resonite.com/Component:AssetReceiver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/82/AssetReceiver%601Component.png/510px-AssetReceiver%601Component.png)](https://wiki.resonite.com/File:AssetReceiver%601Component.png) **Asset Receiver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Asset Receiver is a useful component for getting asset data from a user through a UIX. When this item is placed on a UIX that allows receiving (like a [Button](https://wiki.resonite.com/Component:Button "Component:Button")) and it's `Reference` field is filled, it will be active. When an item is pushed through the canvas where the button is so the interaction laser is hitting it and the item is let go; the value within the field inside of `Reference` is set to the first available [IAsset](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") which is exposed by an [Asset Proxy](https://wiki.resonite.com/Component:AssetProxy "Component:AssetProxy").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") <A>** | The field to fill with a value when a grabbed item with an [Asset Proxy](https://wiki.resonite.com/Component:AssetProxy "Component:AssetProxy") is dropped onto the canvas region with this component. |
| `Undoable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to add changes to this value via grab receiving to the undo stack of the user that changed it. |

Fields
Collapse

## Behavior

## Examples

- [![How to use the Asset Receiver component in a way that will make it do something.](https://wiki.resonite.com/images/thumb/7/7b/AssetRecieverExample.png/148px-AssetRecieverExample.png)](https://wiki.resonite.com/File:AssetRecieverExample.png "How to use the Asset Receiver component in a way that will make it do something.")

How to use the Asset Receiver component in a way that will make it do something.


## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetReceiver&oldid=96532](https://wiki.resonite.com/index.php?title=Component:AssetReceiver&oldid=96532)"

Contents