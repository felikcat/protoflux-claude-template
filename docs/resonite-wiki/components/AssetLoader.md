# Component:AssetLoader

> Source: https://wiki.resonite.com/Component:AssetLoader

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AssetLoader&diff=100132) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/15/AssetLoader%601Component.png/510px-AssetLoader%601Component.png)](https://wiki.resonite.com/File:AssetLoader%601Component.png) **Asset Loader\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

**AssetLoader** is a Component that is used to tell the game that an [Asset](https://wiki.resonite.com/Asset "Asset") is still being used. This is helpful for when an asset is referenced in a way that deletes it during asset cleanup and saving.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Asset` | **A** | The [Asset](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") to keep loaded. |

Fields
Collapse

## Usage

Set the `Asset` field to the [asset](https://wiki.resonite.com/Asset "Asset") that should be kept around, afterwards the asset should not be cleaned up as long as it continues to be referenced by the AssetLoader.

## Examples

Images on fake badges, some UIX elements.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetLoader&oldid=100132](https://wiki.resonite.com/index.php?title=Component:AssetLoader&oldid=100132)"

Contents