# Component:DynamicField

> Source: https://wiki.resonite.com/Component:DynamicField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicField&diff=92586) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/DynamicField%601Component.png/510px-DynamicField%601Component.png)](https://wiki.resonite.com/File:DynamicField%601Component.png) **DynamicField<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicField<T>** binds the [field](https://wiki.resonite.com/Field "Field") pointed to by `TargetField` to the [dynamic variable](https://wiki.resonite.com/Dynamic_variable "Dynamic variable") referred to by `VariableName`. The field must be a [value type](https://wiki.resonite.com/Value_type "Value type").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the dynamic variable to be used |
| `TargetField` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The field that will be used as the dynamic variable's value. |
| `OverrideOnLink` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, the value of the field will be written when this component is moved into a new space |

Fields
Collapse

## Usage

This component works almost exactly like the [DynamicValueVariable](https://wiki.resonite.com/Component:DynamicValueVariable "Component:DynamicValueVariable") component, except that the value used for the dynamic variable is sourced from a separate field. This field will be automatically updated with the value of the dynamic variable, and writing to the field will write to the dynamic variable. This can be used to directly bind fields of separate components as a dynamic variable without having to use a [DynamicValueVariableDriver](https://wiki.resonite.com/Component:DynamicValueVariableDriver "Component:DynamicValueVariableDriver") or similar setup.

## Examples

## See Also

- [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables")
- [Component:DynamicReference](https://wiki.resonite.com/Component:DynamicReference "Component:DynamicReference"), for the same functionality but with [reference types](https://wiki.resonite.com/Reference_types "Reference types").
- [Component:DynamicValueVariable](https://wiki.resonite.com/Component:DynamicValueVariable "Component:DynamicValueVariable")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicField&oldid=92586](https://wiki.resonite.com/index.php?title=Component:DynamicField&oldid=92586)"

Contents