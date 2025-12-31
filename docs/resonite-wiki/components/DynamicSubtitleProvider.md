# Component:DynamicSubtitleProvider

> Source: https://wiki.resonite.com/Component:DynamicSubtitleProvider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9d/DynamicSubtitleProviderComponent.png/510px-DynamicSubtitleProviderComponent.png)](https://wiki.resonite.com/File:DynamicSubtitleProviderComponent.png) **Dynamic Subtitle Provider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicSubtitleProvider** component is used to provide subtitles on videos that are playing in world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `AssetURL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The URI to the subtitle file. |

Fields
Collapse

## Usage

## Examples

Providing a url to this component and using it in an [Animator](https://wiki.resonite.com/Component:Animator "Component:Animator") to drive text synchronized using a [PlaybackSynchronizer](https://wiki.resonite.com/Component:PlaybackSynchronizer "Component:PlaybackSynchronizer") with a video, it can show subtitles.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicSubtitleProvider&oldid=93899](https://wiki.resonite.com/index.php?title=Component:DynamicSubtitleProvider&oldid=93899)"

Contents