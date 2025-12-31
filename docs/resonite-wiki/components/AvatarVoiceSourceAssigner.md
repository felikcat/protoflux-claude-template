# Component:AvatarVoiceSourceAssigner

> Source: https://wiki.resonite.com/Component:AvatarVoiceSourceAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarVoiceSourceAssigner&diff=92257) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1f/AvatarVoiceSourceAssignerComponent.png/510px-AvatarVoiceSourceAssignerComponent.png)](https://wiki.resonite.com/File:AvatarVoiceSourceAssignerComponent.png) **AvatarVoiceSourceAssigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarVoiceSourceAssigner** sets the `IAudioSource` field referenced by `TargetReference` to the voice stream of the active user when the avatar this component is attached to is equipped.

This component is useful when adding voice-driven effects to an avatar, such as a [Component:VisemeAnalyzer](https://wiki.resonite.com/Component:VisemeAnalyzer "Component:VisemeAnalyzer") or [Component:VolumeMeter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter")

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource") >** | Target `IAudioSource` that will be assigned the user's audio stream |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarVoiceSourceAssigner&oldid=92257](https://wiki.resonite.com/index.php?title=Component:AvatarVoiceSourceAssigner&oldid=92257)"

Contents