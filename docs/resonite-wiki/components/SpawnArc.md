# Component:SpawnArc

> Source: https://wiki.resonite.com/Component:SpawnArc

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SpawnArc&diff=98209) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d1/SpawnArcComponent.png/510px-SpawnArcComponent.png)](https://wiki.resonite.com/File:SpawnArcComponent.png) **SpawnArc** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SpawnArc** component spawns in [users](https://wiki.resonite.com/User "User") along the arc of a circle, with an optional weight to select this spawner.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The likelihood of this spawner being chosen for a spawning user. |
| `Capacity` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users this spawner can have spawned at a time. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The range of how far this spawner can spawn this user. |
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The shape of how the spawner will place the user. |
| `UsersPerArc` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The segment area for the users to spawn at in this arc. |
| `CenterArcOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset rotation of the center of the arc circle for this spawner. |
| `GrowBothSides` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The option to extend both sides for the spawn arc, fanning out from a center point. |
| `RowHeightOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The hieght where the users will spawn along the circle. |
| `OrientUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Positions and rotates the user towards the center. |
| `ParentUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Keeps the user parented onto this specific spawner slot. |
| `TiltUsers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Tilts the user when spawning in. |
| `PositionNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | Takes the position of the user's body node for spawning. |
| `RotationNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | Takes the rotation of the user's body node for spawning. |
| `_showTest` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Internal: Mostly for debugging. |
| `_testSlots` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Internal: Shows the number of test slots on this spawning arc. |

Fields
Collapse

## Usage

Used to help shape how you want [users](https://wiki.resonite.com/User "User") to spawn in a [world](https://wiki.resonite.com/World "World").

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SpawnArc&oldid=98209](https://wiki.resonite.com/index.php?title=Component:SpawnArc&oldid=98209)"

Contents