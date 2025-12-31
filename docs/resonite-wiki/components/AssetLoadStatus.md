# Component:AssetLoadStatus

> Source: https://wiki.resonite.com/Component:AssetLoadStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AssetLoadStatus&diff=79025) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/26/AssetLoadStatusComponent.png/510px-AssetLoadStatusComponent.png)](https://wiki.resonite.com/File:AssetLoadStatusComponent.png) **AssetLoadStatus** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Introduction

This is a component that tracks the load status of a list of assets locally.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Assets` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[IAsset](https://wiki.resonite.com/Type:IAsset "Type:IAsset")** | List of assets that the component should listen to for loading status |
| `IsLoaded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Are all the assets in Assets list loaded? |
| `LoadProgress` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ratio of "how many assets are loaded" to the total asset count. |
| `ProgressWeight` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The total count of assets in `Assets`. |

Fields
Collapse

## Behavior

This component returns a ratio of how many of the given assets are actually loaded.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetLoadStatus&oldid=79025](https://wiki.resonite.com/index.php?title=Component:AssetLoadStatus&oldid=79025)"

Contents