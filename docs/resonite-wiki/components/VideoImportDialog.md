# Component:VideoImportDialog

> Source: https://wiki.resonite.com/Component:VideoImportDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f9/VideoImportDialogComponent.png/510px-VideoImportDialogComponent.png)](https://wiki.resonite.com/File:VideoImportDialogComponent.png) **Video Import Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VideoImportDialog** component is better explained in the [Importing](https://wiki.resonite.com/Importing "Importing") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `path` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | A list of sync delegates used to generate the UI when at particular paths in the importer. |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to put ui elements for import options in. |
| `_videoType` | **[VideoImportDialog.VideoType](https://wiki.resonite.com/Component:VideoImportDialog#VideoType)** | The type of video being imported. |
| `_stereoLayout` | **[StereoLayout](https://wiki.resonite.com/Type:StereoLayout "Type:StereoLayout")** | The kind of video stereo layout the video being imported has. |
| `_depthPreset` | **[VideoImportDialog.DepthPreset](https://wiki.resonite.com/Component:VideoImportDialog#DepthPreset)** | The kind of depth the video being imported has. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OpenRoot:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Handles when the dialog is opened to the root menu. |
| `Preset_Video:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports default video. |
| `Preset_360:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports as a 360 video. |
| `Preset_StereoVideo:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports as a default stereo video. |
| `Preset_Stereo360:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports as a stereo 360 video. |
| `Preset_Depth:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports as a depth video. |
| `Preset_180:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports as a 180 video. |
| `Preset_Stereo180:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports as a stereo 180 video. |
| ``MenuStereoLayout:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Switches the menu to show the stereo options. |
| `Preset_HorizontalLR:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports the video as a stereo horizontal Left Right layout. |
| `Preset_HorizontalRL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports the video as a stereo horizontal Right Left layout. |
| `Preset_VerticalLR:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports the video as a stereo vertical Left Right layout. |
| `Preset_VerticalRL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports the video as a stereo vertical Right Left layout. |
| ``MenuDepthPreset:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Switches the menu to show the depth options. |
| `Preset_DepthDefault:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Uses the default depth option. |
| `Preset_DepthPFCapture:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Uses the PF capture vertical depth option. |
| `Preset_DepthPFCaptureHorizontal:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Uses the PF capture horizontal depth option. |
| `Preset_DepthHolofix:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Uses the holofix depth option. |
| `AsRawFile:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Imports the video as a raw file. |
| `Return:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Navigates the menu to the previous menu. |

Triggers
Collapse

## VideoType

| Name | Value | Description |
| --- | --- | --- |
| `Regular` | 0 | Normal video |
| `Sphere360` | 1 | Video is recorded in a 360 equilateral rectangle. |
| `Sphere180` | 2 | Video is recorded in a 180 equilateral rectangle. |
| `Depth` | 3 | The video is recorded with depth data. |

Values

## DepthPreset

| Name | Value | Description |
| --- | --- | --- |
| `Default` | 0 | Uses no depth data. |
| `PFCaptureVertical` | 1 | Says depth is captured vertically where the depth data is below the color data. |
| `PFCaptureHorizontal` | 2 | Says depth is captured horizontally where the depth data is to the left of the color data. |
| `Holofix` | 3 | Depth is Holofixed. |

Values

## Usage

See [Importing](https://wiki.resonite.com/Importing "Importing").

## Examples

See [Importing](https://wiki.resonite.com/Importing "Importing").

## See Also

- [Importing](https://wiki.resonite.com/Importing "Importing")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VideoImportDialog&oldid=100807](https://wiki.resonite.com/index.php?title=Component:VideoImportDialog&oldid=100807)"

Contents