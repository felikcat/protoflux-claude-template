# Component:LocalAudioDeviceStream

> Source: https://wiki.resonite.com/Component:LocalAudioDeviceStream

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/db/LocalAudioDeviceStreamComponent.png/510px-LocalAudioDeviceStreamComponent.png)](https://wiki.resonite.com/File:LocalAudioDeviceStreamComponent.png) **Local Audio Device Stream** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocalAudioDeviceStream** component can be used as a source of streamed audio data kind of like a player or a video for use with audio output components. This component Outputs locally the audio for a specified audio input Device by index number.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AudioDeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The audio device to gather audio samples from. |
| `UseFilteredData` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use raw audio samples or filter them. |

Fields
Collapse

## Usage

Can be used to listen to a specified audio device index using an audio output. Can be used in world space and isn't limited to userspace.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocalAudioDeviceStream&oldid=104616](https://wiki.resonite.com/index.php?title=Component:LocalAudioDeviceStream&oldid=104616)"

Contents