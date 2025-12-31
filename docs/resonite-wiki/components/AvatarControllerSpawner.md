# Component:AvatarControllerSpawner

> Source: https://wiki.resonite.com/Component:AvatarControllerSpawner

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/AvatarControllerSpawnerComponent.png/510px-AvatarControllerSpawnerComponent.png)](https://wiki.resonite.com/File:AvatarControllerSpawnerComponent.png) **Avatar Controller Spawner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarControllerSpawner** component will spawn the corrosponding controller for the user when placed on an avatar under either the right or left hand.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SpawnRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to spawn the model. (The Component attaches a slot called "root" under this when spawning the model, that becomes the model root) |
| `MaterialOverride` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | What material to replace the spawned model's materials with upon spawning. |
| `ControllerSpawned` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"), [User](https://wiki.resonite.com/Type:User "Type:User") >** | The component calls this method when it has finished spawning the model with the user that has this controller model, and the root slot of the spawned model. |
| `_sourceControllerInfo` | **[AvatarControllerInfo](https://wiki.resonite.com/Component:AvatarControllerInfo "Component:AvatarControllerInfo")** | The controller info this component grabbed in order to find and generate the right model. |
| `_lastSpawned` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The froox engine type of the last controller type this component generated. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Can be used to show what kind of controllers the user is using when they get into an avatar.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarControllerSpawner&oldid=95902](https://wiki.resonite.com/index.php?title=Component:AvatarControllerSpawner&oldid=95902)"

Contents