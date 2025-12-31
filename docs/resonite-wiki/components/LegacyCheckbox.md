# Component:LegacyCheckbox

> Source: https://wiki.resonite.com/Component:LegacyCheckbox

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/31/LegacyCheckboxComponent.png/510px-LegacyCheckboxComponent.png)](https://wiki.resonite.com/File:LegacyCheckboxComponent.png) **Legacy Checkbox** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyCheckbox** component is used in old migrated content. This is a Legacy component and should not be used for new content. This should be replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `IsChecked` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the checkbox is checked. |
| `IsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `DriveField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with this checkbooks state. |
| `AllowWriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to the target value of `DriveField` are sent to this component's checked state instead. |
| `Size` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the check box is. |
| `BevelPercent` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How beveled the check box is. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the check box. |
| `_shellMesh` | **[BevelBoxMesh](https://wiki.resonite.com/Component:BevelBoxMesh "Component:BevelBoxMesh")** | The outer shell of the check box. |
| `_checkMesh` | **[BevelBoxMesh](https://wiki.resonite.com/Component:BevelBoxMesh "Component:BevelBoxMesh")** | The inner check box indicator of the check box. |
| `_titleBar` | **[LegacyHorizontalChoiceBar](https://wiki.resonite.com/Component:LegacyHorizontalChoiceBar "Component:LegacyHorizontalChoiceBar")** | unused. |
| `_shellSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the outer shell size mesh. |
| `_shellBevel` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the outer shell bevel. |
| `_checkSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the check indicator size. |
| `_checkBevel` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the check indicator bevel. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the collider size. |
| `_shellMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The field to drive to set the shell material. |
| `_checkMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The field to drive to set the check indicator material. |

Fields
Collapse

## Usage

Just dont.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyCheckbox&oldid=99010](https://wiki.resonite.com/index.php?title=Component:LegacyCheckbox&oldid=99010)"

Contents