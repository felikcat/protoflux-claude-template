# Component:CharacterControllerModifier

> Source: https://wiki.resonite.com/Component:CharacterControllerModifier

!!!ABSTRACT CLASS!!!

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Parameter` | **[CharacterControllerParameter](https://wiki.resonite.com/Type:CharacterControllerParameter "Type:CharacterControllerParameter")** | The parameter to modify. |
| `ModificationMode` | [Mode](https://wiki.resonite.com/Component:CharacterControllerModifier#Mode) | How to modify the parameter. |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `Override` | 0 | Override the original value, replacing it with another value. |
| `Add` | 1 | Add to the original value with another value. |
| `Multiply` | 2 | Multiply the original value with another value. |

Values

## Usage

This is an abstract class used as a base for other components in the code.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterControllerModifier&oldid=94026](https://wiki.resonite.com/index.php?title=Component:CharacterControllerModifier&oldid=94026)"

Contents