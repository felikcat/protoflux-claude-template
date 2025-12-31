# Component:LegacyColorDialog

> Source: https://wiki.resonite.com/Component:LegacyColorDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/24/LegacyColorDialogComponent.png/510px-LegacyColorDialogComponent.png)](https://wiki.resonite.com/File:LegacyColorDialogComponent.png) **Legacy Color Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyColorDialog** component is used in old Legacy content that was migrated and was used to pick colors for color fields. This component should not be used and should be replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Realtime` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component should instantly update the value of the target field in `TargetField` |
| `TargetField` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >>** | The color field this component is editing. |
| `_originalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The original color value `TargetField`'s target field had before editing. |
| `_hue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current selected color hue. |
| `_saturation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current selected color saturation. |
| `_value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current selected color value. |
| `_alpha` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current selected color transparency. |
| `_profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The current selected color profile. |
| `_gain` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current selected color gain. |
| `_rSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | The slider to change the red of the color with. |
| `_gSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | The slider to change the green of the color with. |
| `_bSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | The slider to change the blue of the color with. |
| `_aSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | The slider to change the transparency/alpha of the color with. |
| `_gainSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | The slider to change the gain of the color with. |
| `_rValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the current selected red value. |
| `_gValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the current selected green value. |
| `_bValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the current selected blue value. |
| `_aValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the current selected transparency/alpha value. |
| `_gainValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the current selected gain value. |
| `_colorWheelMesh` | **[ColorWheelTriangleMesh](https://wiki.resonite.com/Component:ColorWheelTriangleMesh "Component:ColorWheelTriangleMesh")** | The triangle color mesh for this UI. |
| `_okButton` | **[LegacyButton](https://wiki.resonite.com/Component:LegacyButton "Component:LegacyButton")** | The button that when pressed applies the selected color and closes the UI. |
| `_cancelButton` | **[LegacyButton](https://wiki.resonite.com/Component:LegacyButton "Component:LegacyButton")** | The button that when pressed reverts the value of the targeted field in `TargetField` to `_originalColor` and closes the ui. |
| `_style` | **[LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle")** | The source of the legacy color styles for this component. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCancelPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Is called when the dialog is canceled. |
| `OnOKPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Is called when "OK" is pressed. |
| `OnPickerTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Is called when the color triangle picker is clicked. |

Triggers
Collapse

## Usage

Just don't.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyColorDialog&oldid=99014](https://wiki.resonite.com/index.php?title=Component:LegacyColorDialog&oldid=99014)"

Contents