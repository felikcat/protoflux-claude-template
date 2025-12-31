# Component:BinaryExportable

> Source: https://wiki.resonite.com/Component:BinaryExportable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BinaryExportable&diff=92438) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/25/BinaryExportableComponent.png/510px-BinaryExportableComponent.png)](https://wiki.resonite.com/File:BinaryExportableComponent.png) **Binary Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BinaryExportable** component takes in a [Binary](https://wiki.resonite.com/Type:Binary "Type:Binary") asset and allows the [Slot](https://wiki.resonite.com/Slot "Slot") to be exportable as a binary file on your device.

This is more of an uncommon way to export your files, but there are a couple of [uses](https://wiki.resonite.com/Component:BinaryExportable#Usage) that are useful to know.

To export using this component, look at the [file browser export section](https://wiki.resonite.com/File_Browser#Importing_And_Exporting "File Browser").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Binary` | **[Binary](https://wiki.resonite.com/Type:Binary "Type:Binary")** | The binary to be exported. |

Fields
Collapse

## Usage

Using this component with the [StaticBinary](https://wiki.resonite.com/Component:StaticBinary "Component:StaticBinary") component, allows the user to export a binary file with a provided [url](https://wiki.resonite.com/Type:Uri "Type:Uri").

Keep in mind that exporting a binary file is one-way currently in [Resonite](https://wiki.resonite.com/Resonite "Resonite") (especially if you are thinking about local storage), this is due to the fact that Resonite uses the `.bin` as files that it does not recognize. So importing from a binary raw file is not doable.

This component is used mainly to add an export option to the user's context menu as they are holding an item. Which can be used to easily communicate to the user that an item is made for exporting to their local machine. For example, screenshots, figurines, pictures, recorded audio clips, some generated text from protoflux, and Avatars can have Asset exportables like this component to signify that they can be downloaded to one's local storage.

## Examples

This component is used as a key component within raw file objects. Which are generated when a user chooses "Raw File" when importing any item.

## See Also

- [Component:ModelExportable](https://wiki.resonite.com/Component:ModelExportable "Component:ModelExportable")
- [Component:PackageExportable](https://wiki.resonite.com/Component:PackageExportable "Component:PackageExportable")
- [Component:TextureExportable](https://wiki.resonite.com/Component:TextureExportable "Component:TextureExportable")
- [Component:AudioExportable](https://wiki.resonite.com/Component:AudioExportable "Component:AudioExportable")
- Component:BinaryExportable
- [Component:VideoExportable](https://wiki.resonite.com/Component:VideoExportable "Component:VideoExportable")
- [Component:TextExportable](https://wiki.resonite.com/Component:TextExportable "Component:TextExportable")
- [Component:VolumeExportable](https://wiki.resonite.com/Component:VolumeExportable "Component:VolumeExportable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BinaryExportable&oldid=92438](https://wiki.resonite.com/index.php?title=Component:BinaryExportable&oldid=92438)"

Contents