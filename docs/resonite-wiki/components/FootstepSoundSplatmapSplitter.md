# Component:FootstepSoundSplatmapSplitter

> Source: https://wiki.resonite.com/Component:FootstepSoundSplatmapSplitter

Collapse **Component image**

[File:FootstepSoundSplatmapSplitterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FootstepSoundSplatmapSplitterComponent.png "File:FootstepSoundSplatmapSplitterComponent.png") **Footstep Sound Splatmap Splitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FootstepSoundSplatmapSplitter** component plays a different sound player depending on what part of a mesh collider on in the same slot a player walks on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SplatMap` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to get channel data from for playing different sound materials. |
| `R_SoundMaterial` | **[IFootstepSoundMaterial](https://wiki.resonite.com/Type:IFootstepSoundMaterial "Type:IFootstepSoundMaterial")** | The sound material to play when the user walks on a part of the mesh collider that maps to the R channel of `SplatMap` |
| `G_SoundMaterial` | **[IFootstepSoundMaterial](https://wiki.resonite.com/Type:IFootstepSoundMaterial "Type:IFootstepSoundMaterial")** | The sound material to play when the user walks on a part of the mesh collider that maps to the G channel of `SplatMap` |
| `B_SoundMaterial` | **[IFootstepSoundMaterial](https://wiki.resonite.com/Type:IFootstepSoundMaterial "Type:IFootstepSoundMaterial")** | The sound material to play when the user walks on a part of the mesh collider that maps to the B channel of `SplatMap` |
| `A_SoundMaterial` | **[IFootstepSoundMaterial](https://wiki.resonite.com/Type:IFootstepSoundMaterial "Type:IFootstepSoundMaterial")** | The sound material to play when the user walks on a part of the mesh collider that maps to the A channel of `SplatMap` |
| `BlendSounds` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to blend sounds together based on what mix of channels the user is stepping on. |
| `MinimumThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum threshold needed for a channel to be for it to cound for a sound. |
| `R_Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength the sound for the R channel has, which can make it have more importance than other channel sounds on the same pixel. |
| `G_Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength the sound for the G channel has, which can make it have more importance than other channel sounds on the same pixel. |
| `B_Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength the sound for the B channel has, which can make it have more importance than other channel sounds on the same pixel. |
| `A_Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength the sound for the A channel has, which can make it have more importance than other channel sounds on the same pixel. |

Fields
Collapse

## Usage

Used to map texture maps for different terrain sections to different noises.

## Examples

Can be used in ports of half-life maps, where the terrain can change from rocky to sandy in the costal maps.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FootstepSoundSplatmapSplitter&oldid=98405](https://wiki.resonite.com/index.php?title=Component:FootstepSoundSplatmapSplitter&oldid=98405)"

Contents