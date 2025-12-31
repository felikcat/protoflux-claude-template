# Component:VideoExportable

> Source: https://wiki.resonite.com/Component:VideoExportable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VideoExportable&diff=92434) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/af/VideoExportableComponent.png/510px-VideoExportableComponent.png)](https://wiki.resonite.com/File:VideoExportableComponent.png) **Video Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VideoExportable** component is used to export a [Video Texture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture") as a video file for your device.

To export using this component, look at the [file browser export section](https://wiki.resonite.com/File_Browser#Importing_And_Exporting "File Browser").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Video` | **[VideoTexture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture")** | The video asset to be exported. |

Fields
Collapse

## Usage

Using this will allow you to export videos. However, only some types of videos can be exported. Videos that were imported from a computer can be exported (`.mp3` and `.mp4` file types). Videos that seem to fail the exporting process are Youtube videos or streaming videos, as they not only fail to export a video file, they instead export a text file (which seems to be html).

This component is used mainly to add an export option to the user's context menu as they are holding an item. Which can be used to easily communicate to the user that an item is made for exporting to their local machine. For example, screenshots, figurines, pictures, recorded audio clips, some generated text from protoflux, and Avatars can have Asset exportables like this component to signify that they can be downloaded to one's local storage.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ModelExportable](https://wiki.resonite.com/Component:ModelExportable "Component:ModelExportable")
- [Component:PackageExportable](https://wiki.resonite.com/Component:PackageExportable "Component:PackageExportable")
- [Component:TextureExportable](https://wiki.resonite.com/Component:TextureExportable "Component:TextureExportable")
- [Component:AudioExportable](https://wiki.resonite.com/Component:AudioExportable "Component:AudioExportable")
- [Component:BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable")
- Component:VideoExportable
- [Component:TextExportable](https://wiki.resonite.com/Component:TextExportable "Component:TextExportable")
- [Component:VolumeExportable](https://wiki.resonite.com/Component:VolumeExportable "Component:VolumeExportable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VideoExportable&oldid=92434](https://wiki.resonite.com/index.php?title=Component:VideoExportable&oldid=92434)"

Contents