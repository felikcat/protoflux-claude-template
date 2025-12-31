# Component:CharacterTeleporter

> Source: https://wiki.resonite.com/Component:CharacterTeleporter

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CharacterTeleporter&diff=98924) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f0/CharacterTeleporterComponent.png/510px-CharacterTeleporterComponent.png)](https://wiki.resonite.com/File:CharacterTeleporterComponent.png) **Character Teleporter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CharacterTeleporter** sets up a Slot to teleport a character to the associated teleport exit when the Slot's Collider is hit. The Collider must be of type Trigger unless `TriggersOnly` is disabled.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TriggersOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only allow triggers in this component's slot hiearchy to trigger the teleporter. |
| `Exits` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[CharacterTeleporter.Exit](https://wiki.resonite.com/Component:CharacterTeleporter#Exit)** | A list of slot exits to send the user to, which include rotation and individualized data. |
| `MinimumVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum velocity the user has to be traveling to enter the teleporter. |
| `DirectionReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which way is looking forward for this teleporter. |
| `MaxDirectionAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If the user's velocity direction has an angle greater than this compared to the `DirectionReference`, then don't teleport the user. |
| `IgnoreParentUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to ignore the active user of this component when finding users that meet the criteria to go through the teleporter. |
| `TeleportEntered` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | [Sync Delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") that take [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") that should be called when the teleporter is entered. For example, [RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer") and [RandomObjectSpawner](https://wiki.resonite.com/Component:RandomObjectSpawner "Component:RandomObjectSpawner") have sync delegates that can be used here. |
| `TeleportExited` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | [Sync Delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") that take [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") that should be called when the teleporter is exited anywhere. For example, [RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer") and [RandomObjectSpawner](https://wiki.resonite.com/Component:RandomObjectSpawner "Component:RandomObjectSpawner") have sync delegates that can be used here. |

Fields
Collapse

## Exit

| Name | Type | Description |
| --- | --- | --- |
| `Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The probability of coming out of this exit. |
| `TeleportExit` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot this exit will send the user to when this exit is chosen. |
| `ParentAfterTeleport` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to parent the character controller slot under `TeleportExit` |
| `TransformRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to rotate the user to align this user to be pointing the same direction relative to this as they were pointing relative to the entrance. |
| `TransformScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to scale the character controller to `TeleportExit`'s scale relative to the entrance. |
| `RelativeExitPoint` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this exit will put the user at the same relative position to it as the user was when they went into the entrance. |
| `RandomExitPointGenerator` | **[IPointGenerator](https://wiki.resonite.com/Type:IPointGenerator "Type:IPointGenerator")** | A generator for points the user should end up when exiting out of this exit. for example, teleporting users into a [circle area](https://wiki.resonite.com/Component:CirclePointGenerator "Component:CirclePointGenerator") after they exit here. Only works if `RelativeExitPoint` is false. |
| `TeleportExitVelocity` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | What velocity to set the user to when they exit out of this exit. |
| `TeleportExited` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | [Sync Delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") that take [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") that should be called when the teleporter is exited here. For example, [RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer") and [RandomObjectSpawner](https://wiki.resonite.com/Component:RandomObjectSpawner "Component:RandomObjectSpawner") have sync delegates that can be used here. |

Fields

## Usage

Place the component on a slot with a collider that has character collider field enabled. Next, specify slot(s) for the user to exit out of in the `Exits` list. Walking into the collider zone will send you and anyone else to the target [Exit](https://wiki.resonite.com/Component:CharacterTeleporter#Exit)

## Examples

Can be used in conjunction with a [Camera Portal](https://wiki.resonite.com/Component:CameraPortal "Component:CameraPortal") to make a gateway/portal. It can also be used to make a Tardis interior.

Teleport users using the CharacterTeleporter component by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime").

![](https://i.ytimg.com/vi/vPj43dD8CQ4/hqdefault.jpg)

[OLD: Neos VR Tutorial: Teleport users using CharacterTeleporter](https://www.youtube-nocookie.com/embed/vPj43dD8CQ4?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

- [RandomObjectSpawner](https://wiki.resonite.com/Component:RandomObjectSpawner "Component:RandomObjectSpawner")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterTeleporter&oldid=98924](https://wiki.resonite.com/index.php?title=Component:CharacterTeleporter&oldid=98924)"

Contents