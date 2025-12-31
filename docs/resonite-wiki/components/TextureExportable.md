# Component:TextureExportable

> Source: https://wiki.resonite.com/Component:TextureExportable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TextureExportable&diff=100741) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fe/TextureExportableComponent.png/510px-TextureExportableComponent.png)](https://wiki.resonite.com/File:TextureExportableComponent.png) **Texture Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureExportable** allows you to make a [StaticTexture2D](https://wiki.resonite.com/StaticTexture2D_(Component) "StaticTexture2D (Component)") exportable through the files page in the [dash menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

To export using this component, look at the [file browser export section](https://wiki.resonite.com/File_Browser#Importing_And_Exporting "File Browser").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to be exported. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `CopyImage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Shows as a button in the user's context menu. Allows copying the image this component points to into the user's clipboard. |

Triggers
Collapse

## Usage

To use this component attach it to an object, than reference a Texture2D in the `Texture` field.

This component is used mainly to add an export option to the user's context menu as they are holding an item. Which can be used to easily communicate to the user that an item is made for exporting to their local machine. For example, screenshots, figurines, pictures, recorded audio clips, some generated text from protoflux, and Avatars can have Asset exportables like this component to signify that they can be downloaded to one's local storage.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ModelExportable](https://wiki.resonite.com/Component:ModelExportable "Component:ModelExportable")
- [Component:PackageExportable](https://wiki.resonite.com/Component:PackageExportable "Component:PackageExportable")
- Component:TextureExportable
- [Component:AudioExportable](https://wiki.resonite.com/Component:AudioExportable "Component:AudioExportable")
- [Component:BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable")
- [Component:VideoExportable](https://wiki.resonite.com/Component:VideoExportable "Component:VideoExportable")
- [Component:TextExportable](https://wiki.resonite.com/Component:TextExportable "Component:TextExportable")
- [Component:VolumeExportable](https://wiki.resonite.com/Component:VolumeExportable "Component:VolumeExportable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureExportable&oldid=100741](https://wiki.resonite.com/index.php?title=Component:TextureExportable&oldid=100741)"

Contents