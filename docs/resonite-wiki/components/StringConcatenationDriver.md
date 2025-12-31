# Component:StringConcatenationDriver

> Source: https://wiki.resonite.com/Component:StringConcatenationDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9c/StringConcatenationDriverComponent.png/510px-StringConcatenationDriverComponent.png)](https://wiki.resonite.com/File:StringConcatenationDriverComponent.png) **String Concatenation Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StringConcatenationDriver** component constructs a string from the inputted list of strings.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetString` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with the resulting completed string. |
| `Separator` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What text to put between each pair of strings when building the string. This can be something like a comma, a space, or anything else the user desires. |
| `Strings` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of strings to join together separated by `Seperator`. |
| `NullOutputWhenAllAreNull` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to null the entire string when all `Strings` fields are null. |

Fields
Collapse

## Usage

Attach to a slot and add a list of strings to `Strings` and a `TargetString` for this to start working.

## Examples

Can be used to automatically construct dynamic variable names without [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"). It can also be used to drive [UIX](https://wiki.resonite.com/UIX "UIX").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StringConcatenationDriver&oldid=95678](https://wiki.resonite.com/index.php?title=Component:StringConcatenationDriver&oldid=95678)"

Contents