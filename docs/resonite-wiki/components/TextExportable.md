# Component:TextExportable

> Source: https://wiki.resonite.com/Component:TextExportable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TextExportable&diff=92439) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/TextExportableComponent.png/510px-TextExportableComponent.png)](https://wiki.resonite.com/File:TextExportableComponent.png) **Text Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextExportable** component allows the user to take a [Slot](https://wiki.resonite.com/Slot "Slot") and export it as a text file on their device.

To export using this component, look at the [file browser export section](https://wiki.resonite.com/File_Browser#Importing_And_Exporting "File Browser").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TextSource` | **[IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Anything that is a string, such as textfields, contents, etc. |
| `Extension` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The file type, defaults to `.txt`. |
| `Description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of what this text export is. Will be shown during the export process. |

Fields
Collapse

## Usage

This can be used to export anything that is text based, or anything you can fill the `TextSource` with such as log information or anything else that you wish to export out.

This component is used mainly to add an export option to the user's context menu as they are holding an item. Which can be used to easily communicate to the user that an item is made for exporting to their local machine. For example, screenshots, figurines, pictures, recorded audio clips, some generated text from protoflux, and Avatars can have Asset exportables like this component to signify that they can be downloaded to one's local storage.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ModelExportable](https://wiki.resonite.com/Component:ModelExportable "Component:ModelExportable")
- [Component:PackageExportable](https://wiki.resonite.com/Component:PackageExportable "Component:PackageExportable")
- [Component:TextureExportable](https://wiki.resonite.com/Component:TextureExportable "Component:TextureExportable")
- [Component:AudioExportable](https://wiki.resonite.com/Component:AudioExportable "Component:AudioExportable")
- [Component:BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable")
- [Component:VideoExportable](https://wiki.resonite.com/Component:VideoExportable "Component:VideoExportable")
- Component:TextExportable
- [Component:VolumeExportable](https://wiki.resonite.com/Component:VolumeExportable "Component:VolumeExportable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextExportable&oldid=92439](https://wiki.resonite.com/index.php?title=Component:TextExportable&oldid=92439)"

Contents