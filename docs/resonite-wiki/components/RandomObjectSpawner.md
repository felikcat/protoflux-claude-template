# Component:RandomObjectSpawner

> Source: https://wiki.resonite.com/Component:RandomObjectSpawner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RandomObjectSpawner&diff=99112) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/6/6a/RandomObjectSpawnerComponent.png)](https://wiki.resonite.com/File:RandomObjectSpawnerComponent.png) **Random Object Spawner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RandomObjectSpawner** component selects a slot from the `Templates` list, and spawns it either at this component's parent (in the case of `Spawn()`), or at the point specified in an argument (in the case of `SpawnAtPoint()`)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Templates` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[RandomObjectSpawner.SpawnData](https://wiki.resonite.com/Component:RandomObjectSpawner#SpawnData)** | List of slots to be selected from, when a Trigger is invoked |
| `SpawnSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space in which the template item will be spawned. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Spawn:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Spawns a slot randomly selected from `Templates`, located at the origin of this component's parent slot. |
| ``SpawnAtPoint:Action`1<Float3>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | X | Spawns a slot randomly selected from `Templates`, located at the provided point. |

Triggers
Collapse

## Behavior

When triggered by any event source that accepts an Action (for `Spawn()`), or Action<float3> (for `SpawnAtPoint()`, this component will spawn a random slot from `Templates`

Prior to [Build 2020.11.8.605](https://discordapp.com/channels/402159838827905024/469131434628612116/774938408870346772), this component would duplicate a random slot from `Templates` in-place, without changing its location.

## Examples

The `Spawn()` trigger can be invoked by a component such as [Button Action Trigger](https://wiki.resonite.com/ButtonActionTrigger_(Component) "ButtonActionTrigger (Component)"), when bound to a [UIX Button](https://wiki.resonite.com/Button_(Component) "Button (Component)") or [Legacy Button](https://wiki.resonite.com/LegacyButton_(Component) "LegacyButton (Component)")

The `SpawnAtPoint()` trigger can be invoked by a component such as [Character Event Trigger](https://wiki.resonite.com/CharacterEventTrigger_(Component) "CharacterEventTrigger (Component)"), which provides the required **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** argument.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RandomObjectSpawner&oldid=99112](https://wiki.resonite.com/index.php?title=Component:RandomObjectSpawner&oldid=99112)"

Contents