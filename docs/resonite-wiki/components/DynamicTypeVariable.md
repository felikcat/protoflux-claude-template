# Component:DynamicTypeVariable

> Source: https://wiki.resonite.com/Component:DynamicTypeVariable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/83/DynamicTypeVariableComponent.png/510px-DynamicTypeVariableComponent.png)](https://wiki.resonite.com/File:DynamicTypeVariableComponent.png) **Dynamic Type Variable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicTypeVariable** Component is used to define a [Type](https://wiki.resonite.com/Type:Type "Type:Type") as the value of a dynamic variable.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable. |
| `Value` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The value of the dynamic variable that keeps in sync with the variable's valye. |
| `OverrideOnLink` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to write the current value of the dynamic variable in a space when it connects to it with the one this component is storing. |

Fields
Collapse

## Usage

For more info on Dynamic Variables and how they work including this type of component, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicTypeVariable&oldid=92446](https://wiki.resonite.com/index.php?title=Component:DynamicTypeVariable&oldid=92446)"

Contents