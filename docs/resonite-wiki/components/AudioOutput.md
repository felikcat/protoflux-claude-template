# Component:AudioOutput

> Source: https://wiki.resonite.com/Component:AudioOutput

Collapse **Component image**

[![](https://wiki.resonite.com/images/f/fc/AudioOutputComponent.png)](https://wiki.resonite.com/File:AudioOutputComponent.png) **Audio Output** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Audio Output is a component that is used to output sound from any kind of IAudioSource. This includes but is not limited to: Audio streams, audio clip players, and voices.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Volume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The volume to play the clip at, from 0 to 1. |
| `Source` | **[IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")** | The source of audio. Can be an [AudioClipPlayer](https://wiki.resonite.com/AudioClipPlayer_(Component) "AudioClipPlayer (Component)"), [LerpingMultiClipPlayer](https://wiki.resonite.com/LerpingMultiClipPlayer_(Component) "LerpingMultiClipPlayer (Component)"), or [MultiAudioClipPlayer](https://wiki.resonite.com/MultiAudioClipPlayer_(Component) "MultiAudioClipPlayer (Component)"). |
| `SpatialBlend` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Blends the the audio between 3D & 2D. |
| `Spatialize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enables or disables rather it's 3D or 2D. |
| `DopplerLevel` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Simulates audio distortion when you or the object is moving. |
| `RolloffMode` | **[AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode")** | Switches between logarithmic and Linear audio falloff. |
| `MinDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Minimum distance you need to be from the source to hear the audio. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum distance from the source until you no longer hear the audio. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | see [Unity audio source priority](https://docs.unity3d.com/ScriptReference/AudioSource-priority.html) |
| `AudioTypeGroup` | **[AudioTypeGroup](https://wiki.resonite.com/Type:AudioTypeGroup "Type:AudioTypeGroup")** | Changes what track of Audio the source should be. SoundEffects, Multimedia, Voice, User Interface. |
| `DistanceSpace` | **[AudioDistanceSpace](https://wiki.resonite.com/Type:AudioDistanceSpace "Type:AudioDistanceSpace")** | Chooses rather the audio should use it's local scale or it's global scale. |
| `MinScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [Min and Max Scale](https://wiki.resonite.com/Component:AudioOutput#Min_and_Max_Scale) |
| `MaxScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [Min and Max Scale](https://wiki.resonite.com/Component:AudioOutput#Min_and_Max_Scale) |
| `IgnoreReverbZones` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If the Audio Source should ignore Reverb Zones. |
| `excludedUsers` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[User](https://wiki.resonite.com/Type:User "Type:User")** | User references placed in here will be excluded from hearing the audio. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``ExludeUser:Action`1<User>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [User](https://wiki.resonite.com/Type:User "Type:User") >** | X | Excludes the User provided to it, so that user cannot hear this audio output. |
| `ExludeLocalUser:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Excludes the local user running this sync method, so they cannot hear this audio output. |
| `RemoveLocalExcludedUser:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | if currently excluded, makes it to where the local user running this sync method is no longer excluded from hearing this audio output. |
| ``RemoveExludedUser:Action`1<User>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [User](https://wiki.resonite.com/Type:User "Type:User") >** | X | If provided user is currently excluded, makes it so that the provided user is no longer excluded from hearing this audio output. |
| `ClearExludedUsers:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Clears all excluded users from the list |
| ``IsUserExluded:Func`2<User, Bool>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [User](https://wiki.resonite.com/Type:User "Type:User"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | X | When provided a user, this function returns whether or not that user is excluded from hearing this audio clip. |

Triggers
Collapse

## Min and Max scale

If `AudioDistanceSpace` is set to Local, then first the scale's XYZ values are averaged. then that number is clamped between `MinScale` and `MaxScale`. Finally `MinDistance` and `MaxDistance` are multipled by the number, and set to the results. Basically scaling min and max distances up/down.

## Usage

Audio Output is used to Output audio from a large variety of audio sources. From Audio Clips, Audio Streams, Opus Streams, etc. Be careful with how many Audio Outputs you have in a world at once or the Audio Buffer can be overfilled and you wont hear anymore Audio Sources until it's cleared. You can negate this by disabling the hierarchy of the Component or the Component itself when it's not in use.

## Examples

In this example. I'm using a [AudioClipPlayer](https://wiki.resonite.com/AudioClipPlayer_(Component) "AudioClipPlayer (Component)") that's going into the Audio Output Source. I set it's volume to .5 so it plays at half volume, disabled DopplerLevel by setting it to 0, changed it's RolloffMode to Linear drop off and made it so you'll only only hear the audio from 5 meters away. I also made it so a specific user can not hear the audio.

[![](https://wiki.resonite.com/images/thumb/1/10/AudioOutputExample.png/500px-AudioOutputExample.png)](https://wiki.resonite.com/File:AudioOutputExample.png)

## See Also

- [Type:IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")
- [ProtoFlux:Play One Shot](https://wiki.resonite.com/ProtoFlux:Play_One_Shot "ProtoFlux:Play One Shot")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioOutput&oldid=97857](https://wiki.resonite.com/index.php?title=Component:AudioOutput&oldid=97857)"

Contents