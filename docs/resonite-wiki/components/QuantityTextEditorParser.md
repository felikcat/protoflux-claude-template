# Component:QuantityTextEditorParser

> Source: https://wiki.resonite.com/Component:QuantityTextEditorParser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/QuantityTextEditorParser%601Component.png/510px-QuantityTextEditorParser%601Component.png)](https://wiki.resonite.com/File:QuantityTextEditorParser%601Component.png) **Quantity Text Editor Parser\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **QuantityTextEditorParser** component takes in a `ParsedValue` and if there is a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") on the same [slot](https://wiki.resonite.com/Slot "Slot"), it will send the value through the text editor and into either a [Text](https://wiki.resonite.com/Component:Text "Component:Text") or a [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer") component.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParseContinuously` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, makes the value always update and parse. If false, it only updates when submitted. |
| `UpdateStringFromValue` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, will update the string value from this parsed value. |
| `ParsedValue` | **T** | The value that was read from the text field. |
| `MinValue` | **T** | The minimum value that can be read. |
| `MaxValue` | **T** | The maximum value that can be read. |
| `IgnoreOutOfRange` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Ignores any value that is out of range from the min and max. |
| `DefaultUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Changes the default unit to show in the text (especially if the `FormatUnit` is incorrect). |
| `FormatUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The unit to show in the text. |
| `FormatNumber` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Formats the string. |
| `CompoundFormatUnits` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Compounds units together (example: feet and inches for height). |
| `CompoundUseLongNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Use the long version of names. |
| `CompoundOverrideNames` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Overrides the names. |
| `CompoundDiscardLastFraction` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Discards the last fraction. |
| `CompoundSeparator` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Separates the compound units. |
| `CompoundZeroHandling` | **[CompoundZeroHandling](https://wiki.resonite.com/Type:CompoundZeroHandling "Type:CompoundZeroHandling")** | Handles zeros for units. |

Fields
Collapse

## Usage

Place on the same [Slot](https://wiki.resonite.com/Slot "Slot") as a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") and anything entered into the text editor will be attempted to be parsed as a [quantity](https://wiki.resonite.com/Quantity_Types "Quantity Types") and output via the `ParsedValue` field.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:QuantityTextEditorParser&oldid=98205](https://wiki.resonite.com/index.php?title=Component:QuantityTextEditorParser&oldid=98205)"

Contents