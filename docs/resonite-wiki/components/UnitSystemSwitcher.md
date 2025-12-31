# Component:UnitSystemSwitcher

> Source: https://wiki.resonite.com/Component:UnitSystemSwitcher

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0e/UnitSystemSwitcherComponent.png/510px-UnitSystemSwitcherComponent.png)](https://wiki.resonite.com/File:UnitSystemSwitcherComponent.png) **Unit System Switcher** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UnitSystemSwitcher** component takes in one [quantity type](https://wiki.resonite.com/Quantity_Types "Quantity Types") and converts it to another as a [string](https://wiki.resonite.com/Type:String "Type:String"). This is commonly used to make editors easily able to take any unit input and automatically know which one the user is referring to.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DefaultUnit` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Changes the default unit to show in the text (especially if the `FormatUnit` is incorrect). |
| `FormatUnit` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The unit to show in the text. |
| `FormatNumber` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Formats the string. |
| `CompoundFormatUnits` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Compounds units together (example: feet and inches for height). |
| `CompoundOverrideNames` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Overrides the names. |
| `CompoundUseLongNames` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether to use long names like "meters" instead of "m". |
| `CompoundSeparator` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Separates the compound units. |
| `DefaultPreset` | _direct_ **[UnitSystemSwitcher.Preset](https://wiki.resonite.com/Component:UnitSystemSwitcher#Preset)** | The default preset. |
| `ImperialPreset` | _direct_ **[UnitSystemSwitcher.Preset](https://wiki.resonite.com/Component:UnitSystemSwitcher#Preset)** | The imperial preset. |

Fields
Collapse

## Preset

| Name | Type | Description |
| --- | --- | --- |
| `DefaultUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The default unit for this unit type. |
| `FormatUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The unit to show in the text. |
| `FormatNumber` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the string. |
| `CompoundFormatUnits` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of compound format units from a unit configuration. |
| `CompoundSeparator` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Separator for compound units for this preset. |
| `CompoundOverrideNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Overrides the names. |
| `CompoundUseLongNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether compound units should use long names (So millimeters vs mm) |

Fields

## Usage

Useful for unit conversions.

## Examples

This component is used in the dash, to display your Height as a [Distance](https://wiki.resonite.com/Type:Distance "Type:Distance") within the right Unit system
(Metric / Imperial)

## See Also

- [Component:QuantityTextFormatDriver](https://wiki.resonite.com/Component:QuantityTextFormatDriver "Component:QuantityTextFormatDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UnitSystemSwitcher&oldid=106603](https://wiki.resonite.com/index.php?title=Component:UnitSystemSwitcher&oldid=106603)"

Contents