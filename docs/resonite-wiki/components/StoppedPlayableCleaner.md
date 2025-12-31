# Component:StoppedPlayableCleaner

> Source: https://wiki.resonite.com/Component:StoppedPlayableCleaner

Collapse **Component image**

[File:StoppedPlayableCleanerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=StoppedPlayableCleanerComponent.png "File:StoppedPlayableCleanerComponent.png") **Stopped Playable Cleaner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Stopped playable cleaner is used on [play one shots](https://wiki.resonite.com/ProtoFlux:Play_One_Shot "ProtoFlux:Play One Shot") in order to delete or clean them once they have finished playing.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Playable` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | the audio player that is playing audio |
| `GracePeriod` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long to wait before deleting the component after it has finished playing. |
| `CheckingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that is monitoring the `Playable` on their machine to check when it has stopped playing |

Fields
Collapse

## Behavior

This component can stop working if the user is AFK or the slot is disabled, and can cause issues in items like boopers and overload the sound buffer.

## Examples

## See Also

- [Play One Shot ProtoFlux Node](https://wiki.resonite.com/ProtoFlux:Play_One_Shot "ProtoFlux:Play One Shot")
- [Audio Clip Player Component](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StoppedPlayableCleaner&oldid=92405](https://wiki.resonite.com/index.php?title=Component:StoppedPlayableCleaner&oldid=92405)"

Contents