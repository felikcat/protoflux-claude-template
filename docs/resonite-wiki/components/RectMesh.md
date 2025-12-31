# Component:RectMesh

> Source: https://wiki.resonite.com/Component:RectMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/32/RectMesh%601Component.png/510px-RectMesh%601Component.png)](https://wiki.resonite.com/File:RectMesh%601Component.png) **Rect Mesh\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RectMesh** component takes in a value (either a dynamic value from an [IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource"), or a min and max [float](https://wiki.resonite.com/Type:Float "Type:Float") value) and parameters for the generated rect mesh, then renders it onto the [UIX](https://wiki.resonite.com/UIX "UIX").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mesh` | _direct_ **M** | The mesh parameters used to render this rect mesh. |
| `Materials` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to render for this rect mesh. |

Fields
Collapse

## Usage

This can be used to make fancy audio visuals from a user's [Audio Stream Controller](https://wiki.resonite.com/Audio_Stream_Controller "Audio Stream Controller").

## Examples

[ProbablePrime's](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime") video tutorial on how to use the [StandaloneRectMesh](https://wiki.resonite.com/Component:StandaloneRectMesh "Component:StandaloneRectMesh") component, as the concept is similar:

![](https://i.ytimg.com/vi/F9_5fp88GUQ/hqdefault.jpg)

[OLD: Neos VR Tutorial: Graphing audio with AudioSourceWaveformMesh](https://www.youtube-nocookie.com/embed/F9_5fp88GUQ?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- Similar to [StandaloneRectMesh](https://wiki.resonite.com/Component:StandaloneRectMesh "Component:StandaloneRectMesh").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RectMesh&oldid=90099](https://wiki.resonite.com/index.php?title=Component:RectMesh&oldid=90099)"

Contents