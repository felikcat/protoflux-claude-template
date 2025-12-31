# Component:VoiceModeSync

> Source: https://wiki.resonite.com/Component:VoiceModeSync

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b0/VoiceModeSyncComponent.png/510px-VoiceModeSyncComponent.png)](https://wiki.resonite.com/File:VoiceModeSyncComponent.png) **VoiceModeSync** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VoiceModeSync** component only works in [userspace](https://wiki.resonite.com/Userspace "Userspace"). It allows for getting the status of the user's chosen voice mode options and if they can use certain modes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FocusedWorldVoiceMode` | **[VoiceMode](https://wiki.resonite.com/Type:VoiceMode "Type:VoiceMode")** | The voice mode set for the current world. |
| `GlobalMute` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is muted for everyone. |
| `FocusedWorldMaxAllowedVoiceMode` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[VoiceMode](https://wiki.resonite.com/Type:VoiceMode "Type:VoiceMode")** | The maximum voice mode their allowed by the role the user has in the current focused world. |
| `BroadcastAllowed` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether broadcast is allowed for the user voice modes for the user in the currently focused world. |
| `ShoutAllowed` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether shout is allowed for the user voice modes for the user in the currently focused world. |
| `NormalAllowed` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether normal is allowed for the user voice modes for the user in the currently focused world. |
| `WhisperAllowed` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether whisper is allowed for the user voice modes for the user in the currently focused world. |

Fields
Collapse

## Usage

Attach to a slot that would exist in [userspace](https://wiki.resonite.com/Userspace "Userspace"), such as a [facet](https://wiki.resonite.com/Facet "Facet"). From there, the fields will update depending on the currently focused world.

## Examples

Used in the default microphone modes facet.

## See Also

- [Userspace](https://wiki.resonite.com/Userspace "Userspace")
- [Dash menu](https://wiki.resonite.com/Dash_menu "Dash menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VoiceModeSync&oldid=100125](https://wiki.resonite.com/index.php?title=Component:VoiceModeSync&oldid=100125)"

Contents