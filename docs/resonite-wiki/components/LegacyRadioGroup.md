# Component:LegacyRadioGroup

> Source: https://wiki.resonite.com/Component:LegacyRadioGroup

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e5/LegacyRadioGroupComponent.png/510px-LegacyRadioGroupComponent.png)](https://wiki.resonite.com/File:LegacyRadioGroupComponent.png) **Legacy Radio Group** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyRadioGroup** component was used to manage multiple [Legacy Radios](https://wiki.resonite.com/Component:LegacyRadio "Component:LegacyRadio") as part of a list of exclusive options. This component is a part of migrated content and should not be used in new content. This component should be replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `IsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `_selectedOption` | **[LegacyRadio](https://wiki.resonite.com/Component:LegacyRadio "Component:LegacyRadio")** | The Legacy Radio this component has as the chosen option. |
| `_choiceVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot of the choice check mark. |
| `_choicePosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to position the check mark. |
| `_choiceRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the check mark's rotation. |
| `_choiceScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the check mark's scale. |
| `_choiceMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the check mark visual. |

Fields
Collapse

## Usage

Just dont.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:LegacyRadio](https://wiki.resonite.com/Component:LegacyRadio "Component:LegacyRadio")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyRadioGroup&oldid=99028](https://wiki.resonite.com/index.php?title=Component:LegacyRadioGroup&oldid=99028)"

Contents