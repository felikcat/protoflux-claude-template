# Component:ScaleObjectManager

> Source: https://wiki.resonite.com/Component:ScaleObjectManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScaleObjectManager&diff=106625) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/86/ScaleObjectManagerComponent.png/510px-ScaleObjectManagerComponent.png)](https://wiki.resonite.com/File:ScaleObjectManagerComponent.png) **Scale Object Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleObjectManager** component is used to create a field of objects with different relative sizes. This is used most prominently in the "Size of the Universe Adventure" world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ScalePower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `LowerBound` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `UpperBound` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `FarSizeTransitionRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `FarSizeTransitionExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `NearSizeTransitionRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `NearSizeTransitionExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `FarOffsetTransitionRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `FarOffsetTransitionExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `FarTransitionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |
| `NearOffsetTransitionRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `NearOffsetTransitionExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `NearTransitionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |
| `CenterOffsetRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `OptimalDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `CoordinatePowerBase` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnPlaceAtOptimalDistance:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Place At Optimal Distance button is touched. |
| `ResetFarAwayObjects:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Reset Far Away Objects button is touched. |
| `OnRandomizeLocations:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Randomize Locations button is touched. |
| `AlignAll:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Align All button is touched. |
| `OnGenerateTestObjects:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Generate Test Objects button is touched. |
| `UpdateAll:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Update All button is touched. |

Triggers
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleObjectManager&oldid=106625](https://wiki.resonite.com/index.php?title=Component:ScaleObjectManager&oldid=106625)"

Contents