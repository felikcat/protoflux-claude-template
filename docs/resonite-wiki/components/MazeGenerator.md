# Component:MazeGenerator

> Source: https://wiki.resonite.com/Component:MazeGenerator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/95/MazeGeneratorComponent.png/510px-MazeGeneratorComponent.png)](https://wiki.resonite.com/File:MazeGeneratorComponent.png) **Maze Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MazeGenerator** component generates a maze (with a ton of [slots](https://wiki.resonite.com/Slot "Slot")) with given parameters.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Seed` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The random seed for generating this maze. |
| `Cells` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The maze square sections for this generated maze. |
| `WallSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | X: how long the walls are, Y: how tall the walls are. |
| `Point0` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The start position for this maze. |
| `Point1` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The end position for this maze. |
| `Material` | **[MaterialProvider](https://wiki.resonite.com/index.php?title=Type:MaterialProvider&action=edit&redlink=1 "Type:MaterialProvider (page does not exist)")** | The material for the walls of the maze. |
| `Bake` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Bakes the generated maze. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Generate:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Generate the maze. |
| `OnRandomizeSeed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the randomize seed button is touched. |
| `OnGenerate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the generate button is touched. |

Triggers
Collapse

## Usage

Great for prototyping mazes, and can be baked.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MazeGenerator&oldid=99071](https://wiki.resonite.com/index.php?title=Component:MazeGenerator&oldid=99071)"

Contents