# Component:QuantityTextFormatDriver

> Source: https://wiki.resonite.com/Component:QuantityTextFormatDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d8/QuantityTextFormatDriver%601Component.png/510px-QuantityTextFormatDriver%601Component.png)](https://wiki.resonite.com/File:QuantityTextFormatDriver%601Component.png) **Quantity Text Format Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The QuantityTextFormatDriver allows driving a string with an auto formatted quantity.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with the formatted Quantity string. |
| `BaseValue` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | Value to get converted into string |
| `FormatUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Unit to format BaseValue in. |
| `FormatNumber` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the number when making it part of the string (So if it should remove decimals. |
| `CompoundFormatUnits` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of format Units this can use to format the base value (common ones are "ft" as an entry followed by another entry with "in" or "m" as an entry followed by another entry with "cm" ). |
| `CompoundUseLongNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show the long names of compound units. |
| `CompoundOverrideNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the compound format unit names should be used rather than their usual name. |
| `CompoundDiscardLastFraction` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to discard the decimal of the smallest unit being displayed in the output or not. (so "3m 2.5cm" will become 3m 2cm") |
| `CompoundSeparator` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | String to put between compound units. |
| `CompoundZeroHandling` | **[CompoundZeroHandling](https://wiki.resonite.com/Type:CompoundZeroHandling "Type:CompoundZeroHandling")** | Remove or trim compound units with a value of zero. |

Fields
Collapse

## Behavior

The most suitable unit type is automatically chosen based on the BaseValue, you can override this behavior by inputting a unit type into FormatUnit or using compound units.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:QuantityTextFormatDriver&oldid=99170](https://wiki.resonite.com/index.php?title=Component:QuantityTextFormatDriver&oldid=99170)"

Contents