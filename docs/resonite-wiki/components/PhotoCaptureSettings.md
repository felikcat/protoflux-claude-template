# Component:PhotoCaptureSettings

> Source: https://wiki.resonite.com/Component:PhotoCaptureSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7d/PhotoCaptureSettingsComponent.png/510px-PhotoCaptureSettingsComponent.png)](https://wiki.resonite.com/File:PhotoCaptureSettingsComponent.png) **Photo Capture Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PhotoCaptureSettings** component is used to control the behavior of the [PhotoCaptureManager](https://wiki.resonite.com/Component:PhotoCaptureManager "Component:PhotoCaptureManager") and what it does.

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FingerGestureEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the finger photos should even render. |
| `NormalCaptureResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution of pictures taken without timer. |
| `TimerCaptureResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution of pictures taken with timer. |
| `TimerSeconds` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the timer should be for timed photos. |
| `CapturePrivateUI` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether finger photos should capture private ui elements like the dash. |
| `CaptureStereo` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether photos should be 3D with a left and right "eye". |
| `StereoSeparation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how far apart the left and right "eye" are when taking stereo photos. |
| `AlwaysHideNameplates` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to always hide nameplates in taken photos. |
| `EncodeFormat` | **[PhotoEncodeFormat](https://wiki.resonite.com/Type:PhotoEncodeFormat "Type:PhotoEncodeFormat")** | The format taken photos should output as. |
| `PhotoAutosavePath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Where to auto save photos in the inventory to. |
| `AutosaveActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the auto save photos to inventory feature. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OpenAutosavePath:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Opens the auto save path set in the settings. |

Triggers
Collapse

## Usage

## Examples

## See Also

- [Component:PhotoCaptureManager](https://wiki.resonite.com/Component:PhotoCaptureManager "Component:PhotoCaptureManager")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PhotoCaptureSettings&oldid=106249](https://wiki.resonite.com/index.php?title=Component:PhotoCaptureSettings&oldid=106249)"

Contents