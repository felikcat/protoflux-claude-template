# Component:DynamicValueVariableDriver

> Source: https://wiki.resonite.com/Component:DynamicValueVariableDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicValueVariableDriver&diff=98438) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cc/DynamicValueVariableDriver%601Component.png/510px-DynamicValueVariableDriver%601Component.png)](https://wiki.resonite.com/File:DynamicValueVariableDriver%601Component.png) **Dynamic Value Variable Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Dynamic Value Variable Driver is a component that can drive a [IField\`1 (Value Holder)](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") to the value assigned to a dynamic variable with the name `VariableName`. if the specified variable cannot be found, the value will revert to `DefaultTarget` how this works is explained on [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Variable name that will be used to link this component's refrenced value to the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The value/reference to revert to when this component cannot find the specified `VariableName` dynamic variable. |
| `DefaultValue` | **T** | The value to revert to when one doesn't exist. |

Fields
Collapse

## Usage

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicValueVariableDriver&oldid=98438](https://wiki.resonite.com/index.php?title=Component:DynamicValueVariableDriver&oldid=98438)"

Contents