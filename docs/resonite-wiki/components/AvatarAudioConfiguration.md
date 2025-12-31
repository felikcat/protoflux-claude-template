# Component:AvatarAudioConfiguration

> Source: https://wiki.resonite.com/Component:AvatarAudioConfiguration

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b2/AvatarAudioConfigurationComponent.png/510px-AvatarAudioConfigurationComponent.png)](https://wiki.resonite.com/File:AvatarAudioConfigurationComponent.png) **AvatarAudioConfiguration** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Audio Configuration is a component that allows for overriding [Avatar Audio Output Manager](https://wiki.resonite.com/Component:AvatarAudioOutputManager "Component:AvatarAudioOutputManager") voice configs in worlds using user injection.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Normal` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | The settings to override `NormalConfig` on an [Avatar Audio Output Manager](https://wiki.resonite.com/Component:AvatarAudioOutputManager "Component:AvatarAudioOutputManager") with. |
| `Shout` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | The settings to override `ShoutConfig` on an [Avatar Audio Output Manager](https://wiki.resonite.com/Component:AvatarAudioOutputManager "Component:AvatarAudioOutputManager") with. |
| `Broadcast` | _direct_ **[VoiceModeConfig](https://wiki.resonite.com/Type:VoiceModeConfig "Type:VoiceModeConfig")** | The settings to override `BroadcastConfig` on an [Avatar Audio Output Manager](https://wiki.resonite.com/Component:AvatarAudioOutputManager "Component:AvatarAudioOutputManager") with. |

Fields
Collapse

## Usage

attach this component as part of the hierarchy of a slot that is put into `AutoInject` on a [Common Avatar Builder Component](https://wiki.resonite.com/Component:CommonAvatarBuilder "Component:CommonAvatarBuilder") on the world root. When the component is injected, it will auto fill itself into the `_audioConfiguration` of the user's [Avatar Audio Output Manager](https://wiki.resonite.com/Component:AvatarAudioOutputManager "Component:AvatarAudioOutputManager") and allow for overriding the user's audio config.

## Examples

This can be used to make a world system where if a user is in a different room than you, their voice will automatically silence locally for you, so you cannot hear them. This can be useful for making sound proof rooms. The opposite can be done, where a user going up to a microphone on a stand in a world will make their voice global for everyone, or only for people in a room for the speaker that microphone controls.

This can also be used to make a world system where voices are culled depending on where you look as well. which can act like a world-sided Earmuffs mode like the one in settings.

## Related Components

- For how world injected modules work (which said injected slot can contain this component) see [Common Avatar Builder Component](https://wiki.resonite.com/Component:CommonAvatarBuilder "Component:CommonAvatarBuilder")
- For the component this overrides for user voices, see [Avatar Audio Output Manager](https://wiki.resonite.com/Component:AvatarAudioOutputManager "Component:AvatarAudioOutputManager").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarAudioConfiguration&oldid=91599](https://wiki.resonite.com/index.php?title=Component:AvatarAudioConfiguration&oldid=91599)"

Contents