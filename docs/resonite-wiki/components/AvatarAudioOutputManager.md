# Component:AvatarAudioOutputManager

> Source: https://wiki.resonite.com/Component:AvatarAudioOutputManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarAudioOutputManager&diff=91598) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f5/AvatarAudioOutputManagerComponent.png/510px-AvatarAudioOutputManagerComponent.png)](https://wiki.resonite.com/File:AvatarAudioOutputManagerComponent.png) **AvatarAudioOutputManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Audio Output Manager is the component that handles changing the audio output values when a user changes their voice mode or mutes.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AudioOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output this component is controlling and targeting that has the `_activeUser`'s voice. |
| `IsViewVoice` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not this component is the voice of the `_activeUser`'s head or the `_activeUser`'s free cam. |
| `WhisperConfig` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | What `AudioOutput` should be set to when `_activeUser` is in Whisper voice mode. |
| `NormalConfig` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | What `AudioOutput` should be set to when `_activeUser` is in Normal voice mode. |
| `ShoutConfig` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | What `AudioOutput` should be set to when `_activeUser` is in Shout voice mode. |
| `BroadcastConfig` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | What `AudioOutput` should be set to when the user is in Broadcast mode. |
| `__legacyWhisperVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `__legacyNormalVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `__legacyShoutVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `__legacyBroadcastVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `__legacyNormalDopplerLevel` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `__legacyShoutDopplerLevel` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `__legacyWhisperRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal. |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that this component is supposed to be managing an [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") for. |
| `_enabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_volume` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The volume field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_doppler` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The doppler field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_spatialize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The spatialize field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_spatialBlend` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The spatialBlend field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_minDistance` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minDistance field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_maxDistance` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maxDistance field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_rollOffMode` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode")** | The rollOffMode field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_distanceSpace` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[AudioDistanceSpace](https://wiki.resonite.com/Type:AudioDistanceSpace "Type:AudioDistanceSpace")** | The distance space field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_minScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minScale field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_maxScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maxScale field of the [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") controlled by this component. |
| `_scaleCompensation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the volume range of the user so a small `_activeUser` can still be heard by everyone else. |
| `_audioConfiguration` | **[AvatarAudioConfiguration](https://wiki.resonite.com/Component:AvatarAudioConfiguration "Component:AvatarAudioConfiguration")** | A field automatically filled with an Avatar Audio Configuration when the user spawns with an injected Avatar Audio Configuration courtesy of the world they spawned in. When not null, the specified component overrides `WhisperConfig`, `NormalConfig`, `ShoutConfig`, and `BroadcastConfig` voice settings. |

Fields
Collapse

## Behavior

## Examples

## Related Components

- For how to override the user's voice settings in a world, see the [Avatar Audio Configuration Component](https://wiki.resonite.com/Component:AvatarAudioConfiguration "Component:AvatarAudioConfiguration").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarAudioOutputManager&oldid=91598](https://wiki.resonite.com/index.php?title=Component:AvatarAudioOutputManager&oldid=91598)"

Contents