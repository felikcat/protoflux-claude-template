# Component:DynamicTypeField

> Source: https://wiki.resonite.com/Component:DynamicTypeField

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/39/DynamicTypeFieldComponent.png/510px-DynamicTypeFieldComponent.png)](https://wiki.resonite.com/File:DynamicTypeFieldComponent.png) **Dynamic Type Field** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicTypeField** Component is used to mark a field containing a [Type](https://wiki.resonite.com/Type:Type "Type:Type") as the value of a dynamic variable.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable. |
| `TargetField` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType") >** | The field to stay up to date with and change the value of the dynamic variable's value. |
| `OverrideOnLink` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to write the current value of the dynamic variable in a space when it connects to it with the one this component is storing. |

Fields
Collapse

## Usage

For more info on Dynamic Variables and how they work including this type of component, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicTypeField&oldid=92445](https://wiki.resonite.com/index.php?title=Component:DynamicTypeField&oldid=92445)"

Contents