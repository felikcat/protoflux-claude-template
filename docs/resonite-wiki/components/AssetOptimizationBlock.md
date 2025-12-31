# Component:AssetOptimizationBlock

> Source: https://wiki.resonite.com/Component:AssetOptimizationBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AssetOptimizationBlock&diff=98513) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ec/AssetOptimizationBlockComponent.png/510px-AssetOptimizationBlockComponent.png)](https://wiki.resonite.com/File:AssetOptimizationBlockComponent.png) **Asset Optimization Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AssetOptimizationBlock** component is used to prevent the asset optimization tasks in the game from [slots](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") by this component.
Currently according to decompiled code as of 13/10/2024, asset optimization block just prevents materials on the same slot that are the same value wise from being merged.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

## Examples

Usually put on freshly imported assets so materials don't get merged while the user is working on them. This is in case that the materials don't have textures and a bunch of them have the same color.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetOptimizationBlock&oldid=98513](https://wiki.resonite.com/index.php?title=Component:AssetOptimizationBlock&oldid=98513)"

Contents