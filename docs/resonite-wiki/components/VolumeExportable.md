# Component:VolumeExportable

> Source: https://wiki.resonite.com/Component:VolumeExportable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6d/VolumeExportableComponent.png/510px-VolumeExportableComponent.png)](https://wiki.resonite.com/File:VolumeExportableComponent.png) **Volume Exportable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VolumeExportable** component is used to export [3D textures](https://wiki.resonite.com/Texture3D "Texture3D") (or 2D images that a layered on top of each other) as a `.cube` file format.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Volume` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The 3D Texture to be exported. |

Fields
Collapse

## Usage

This is used to make 3D images, 3D scans, 3D volumes, and 3D textures. This can be made outside of [Resonite](https://wiki.resonite.com/Resonite "Resonite") using an external program, or can be made inside Resonite using procedural meshes and components such as [UVW\_ProceduralTexture3D](https://wiki.resonite.com/Component:UVW_ProceduralTexture3D "Component:UVW ProceduralTexture3D"), [FogBoxVolumeMaterial](https://wiki.resonite.com/Component:FogBoxVolumeMaterial "Component:FogBoxVolumeMaterial"), and [VolumeUnlitMaterial](https://wiki.resonite.com/Component:VolumeUnlitMaterial "Component:VolumeUnlitMaterial").

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you can't see what this is exporting, you can always make a box and use the [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") and apply the 3D Texture material to it.


When [importing a Texture3D](https://wiki.resonite.com/3D_Texture_Import "3D Texture Import"), it will be pre-setup and organized for you automatically, also allowing you to export it once more.

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
- [Component:TextExportable](https://wiki.resonite.com/Component:TextExportable "Component:TextExportable")
- Component:VolumeExportable

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VolumeExportable&oldid=113616](https://wiki.resonite.com/index.php?title=Component:VolumeExportable&oldid=113616)"

Contents