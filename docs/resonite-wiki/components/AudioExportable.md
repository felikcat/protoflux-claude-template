# Component:AudioExportable

> Source: https://wiki.resonite.com/Component:AudioExportable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioExportable&diff=92437) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bf/AudioExportableComponent.png/510px-AudioExportableComponent.png)](https://wiki.resonite.com/File:AudioExportableComponent.png) **Audio Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioExportable** component is used to export an [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") as a file for your device.

To export using this component, look at the [file browser export section](https://wiki.resonite.com/File_Browser#Importing_And_Exporting "File Browser").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Audio` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to be exported. |

Fields
Collapse

## Usage

Is used to make an item export an audio clip when a user tries to export the root object.

This component is used mainly to add an export option to the user's context menu as they are holding an item. Which can be used to easily communicate to the user that an item is made for exporting to their local machine. For example, screenshots, figurines, pictures, recorded audio clips, some generated text from protoflux, and Avatars can have Asset exportables like this component to signify that they can be downloaded to one's local storage.

## Examples

Default audio clip players use this component so you export the audio, rather than the player as a bunch of empty objects or a 3D model.

## See Also

- [Component:ModelExportable](https://wiki.resonite.com/Component:ModelExportable "Component:ModelExportable")
- [Component:PackageExportable](https://wiki.resonite.com/Component:PackageExportable "Component:PackageExportable")
- [Component:TextureExportable](https://wiki.resonite.com/Component:TextureExportable "Component:TextureExportable")
- Component:AudioExportable
- [Component:BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable")
- [Component:VideoExportable](https://wiki.resonite.com/Component:VideoExportable "Component:VideoExportable")
- [Component:TextExportable](https://wiki.resonite.com/Component:TextExportable "Component:TextExportable")
- [Component:VolumeExportable](https://wiki.resonite.com/Component:VolumeExportable "Component:VolumeExportable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioExportable&oldid=92437](https://wiki.resonite.com/index.php?title=Component:AudioExportable&oldid=92437)"

Contents