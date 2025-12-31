# Component:PackageExportable

> Source: https://wiki.resonite.com/Component:PackageExportable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/49/PackageExportableComponent.png/510px-PackageExportableComponent.png)](https://wiki.resonite.com/File:PackageExportableComponent.png) **Package Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PackageExportable** component takes in any [Slot](https://wiki.resonite.com/Slot "Slot") hierarchy as a field, and when the slot that has this exportable component on it gets exported, it will actually save a file on your device of the target slot hierarchy provided (and not the item that your exporting from unless it is also under that hierarchy).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot hierarchy to be exported. |

Fields
Collapse

## Usage

This can be a better alternative than using the [BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable") for storage of assets, items, or worlds.

This component is used mainly to add an export option to the user's context menu as they are holding an item. Which can be used to easily communicate to the user that an item is made for exporting to their local machine. For example, screenshots, figurines, pictures, recorded audio clips, some generated text from protoflux, and Avatars can have Asset exportables like this component to signify that they can be downloaded to one's local storage.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ModelExportable](https://wiki.resonite.com/Component:ModelExportable "Component:ModelExportable")
- Component:PackageExportable
- [Component:TextureExportable](https://wiki.resonite.com/Component:TextureExportable "Component:TextureExportable")
- [Component:AudioExportable](https://wiki.resonite.com/Component:AudioExportable "Component:AudioExportable")
- [Component:BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable")
- [Component:VideoExportable](https://wiki.resonite.com/Component:VideoExportable "Component:VideoExportable")
- [Component:TextExportable](https://wiki.resonite.com/Component:TextExportable "Component:TextExportable")
- [Component:VolumeExportable](https://wiki.resonite.com/Component:VolumeExportable "Component:VolumeExportable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PackageExportable&oldid=92435](https://wiki.resonite.com/index.php?title=Component:PackageExportable&oldid=92435)"

Contents