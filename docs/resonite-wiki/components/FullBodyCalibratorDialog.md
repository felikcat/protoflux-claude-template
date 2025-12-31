# Component:FullBodyCalibratorDialog

> Source: https://wiki.resonite.com/Component:FullBodyCalibratorDialog

Collapse **Component image**

[File:FullBodyCalibratorDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FullBodyCalibratorDialogComponent.png "File:FullBodyCalibratorDialogComponent.png") **Full Body Calibrator Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_calibrator` | **[FullBodyCalibrator](https://wiki.resonite.com/Component:FullBodyCalibrator "Component:FullBodyCalibrator")** | The current calibrator this dialog is linked to. |
| `_currentPage` | **[FullBodyCalibratorDialog.Page](https://wiki.resonite.com/Component:FullBodyCalibratorDialog#Page)** | The current dialog page this is showing. |
| `_confirmTrackers` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to confirm trackers. |
| `_resetTrackers` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to reset tracker mappings. |
| `_calibrateAvatar` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to start avatar calibration |
| `_heightCompensation` | **[Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | How much to scale up the avatar to fit the user. |
| `_useSymmetry` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether changes to sided points (left versus right) mirror onto the other side. |
| `_showBodyOverlay` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether to show the invisible person Overlay. |
| `_showAvatarOverlay` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether to show a copy of the avatar on the pedestal. |
| `_hipsMapping` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to indicate if hips are mapped or not. |
| `_feetMapping` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to indicate if feet are mapped or not. |
| `_chestMapping` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to indicate if chest is mapped or not. |
| `_elbowsMapping` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to indicate if elbows are mapped or not. |
| `_kneesMapping` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to indicate if knees are mapped or not. |
| `_heightField` | **[QuantityTextEditorParser\`2](https://wiki.resonite.com/Component:QuantityTextEditorParser%602 "Component:QuantityTextEditorParser`2") < [Distance](https://wiki.resonite.com/Type:Distance "Type:Distance"), [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The text field that changes your user height setting on the fly. |
| `_heightWarning` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to warn if the height is improper. |
| `_useImperial` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the height should be interpreted in yee haw (imperal height). |
| `_swapRegion` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | The component that handles transitions from one page to another on the dialog. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnStartCalibration:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses start calibration. |
| `OnResetTrackers:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses reset trackers. |
| `OnCalibrateAvatar:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses calibrate my avatar. |
| `OnResetAvatarMapping:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses Reset avatar mapping. |
| `OnResetAvatarHeightCompensation:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses Reset avatar height compensation. |
| `OnFinishAvatarCalibration:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses Finish avatar calibration. |
| `OnCloseCalibrator:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user closes the calibrator. |
| `OnReturnToTrackerCalibration:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user presses return to tracker calibration. |

Triggers
Collapse

## Page

| Name | Value | Description |
| --- | --- | --- |
| `MappingTrackers` | 0 | The dialog is on the Mapping Trackers page. |
| `CalibratingTPose` | 1 | The dialog is on the Calibrating T-Pose page. |
| `CalibratingTrackers` | 2 | The dialog is on the Calibrating Trackers page. |
| `CalibratingAvatar` | 3 | The dialog is on the Calibrating Avatar page. |
| `CalibrationFinished` | 4 | The dialog is on the Finish Calibration page. |

Values

## Usage

See [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking").

## Examples

See [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking").

## See Also

- [Full Body Tracking](https://wiki.resonite.com/Full_Body_Tracking "Full Body Tracking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FullBodyCalibratorDialog&oldid=98407](https://wiki.resonite.com/index.php?title=Component:FullBodyCalibratorDialog&oldid=98407)"

Contents