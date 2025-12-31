# Component:ImageImportDialog

> Source: https://wiki.resonite.com/Component:ImageImportDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/99/ImageImportDialogComponent.png/510px-ImageImportDialogComponent.png)](https://wiki.resonite.com/File:ImageImportDialogComponent.png) **Image Import Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Image Import](https://wiki.resonite.com/Image_Import "Image Import").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `path` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | A list of sync delegates used to generate the UI when at particular paths in the importer. |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to put ui elements for import options in. |
| `_projection` | **[ImageProjection](https://wiki.resonite.com/Type:ImageProjection "Type:ImageProjection")** | What image projection to import the image as. |
| `_layout` | **[StereoLayout](https://wiki.resonite.com/Type:StereoLayout "Type:StereoLayout")** | The image stereo layout for left and right to use. |
| `_screenshot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to import the image as a screenshot. |
| `_pointFiltering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the image as pixel art or not. |
| `_uncompressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the image as uncompressed or not. |
| `_alphaBleed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the image with alpha bleed reduction or not. |
| `_lut` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this image is a [Look Up Table](https://wiki.resonite.com/Component:StaticTexture3D "Component:StaticTexture3D"). |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OpenRoot:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Go back to the root screen. |
| `Preset_Image:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Image preset. |
| `Preset_Screenshot:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Screenshot preset. |
| `Preset_PixelArt:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Pixel Art preset. |
| `Preset_Sprite:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Sprite preset. |
| `Preset_360:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the 360 or skybox preset. |
| `Preset_StereoImage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Stereo Image preset. |
| `Preset_Stereo360:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Stereo 360 or depth skybox preset. |
| `Preset_180:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the 180 preset. |
| `Preset_Stereo180:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Stereo 180 preset. |
| `Preset_LUT:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the [Look Up Table](https://wiki.resonite.com/Component:StaticTexture3D "Component:StaticTexture3D") preset. |
| ``MenuStereoLayout:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Go to the import image as stereo menu. |
| `Preset_HorizontalLR:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Horizontal Left Right Stereo image/depth image preset. |
| `Preset_HorizontalRL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Horizontal Right Left Stereo image/depth image preset. |
| `Preset_VerticalLR:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Vertical Left Right Stereo image/depth image preset. |
| `Preset_VerticalRL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use the Vertical Right Left Stereo image/depth image preset. |
| `AsRawFile:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Import the image as a raw file. |
| `Return:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Go back in the menus. |

Triggers
Collapse

## Usage

See [Image Import](https://wiki.resonite.com/Image_Import "Image Import").

## Examples

See [Image Import](https://wiki.resonite.com/Image_Import "Image Import").

## See Also

- [Image Import](https://wiki.resonite.com/Image_Import "Image Import")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ImageImportDialog&oldid=98458](https://wiki.resonite.com/index.php?title=Component:ImageImportDialog&oldid=98458)"

Contents