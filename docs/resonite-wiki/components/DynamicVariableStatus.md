# Component:DynamicVariableStatus

> Source: https://wiki.resonite.com/Component:DynamicVariableStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicVariableStatus&diff=93429) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d8/DynamicVariableStatus%601Component.png/510px-DynamicVariableStatus%601Component.png)](https://wiki.resonite.com/File:DynamicVariableStatus%601Component.png) **Dynamic Variable Status\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Dynamic Variable Status is a component that allows for reading if a certain [dynamic variable](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") with a type and name exists and/or is linked to a [space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace"). Which space this component reads from is determined by the slot this component is attached to. How a slot finds a dynamic variable space is further explained on the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Variable name to check the status for with the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. |
| `IsLinkedToSpace` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Checks if the variable with the `VariableName` and with this component's sub type (the "<T>" of this component) is linked to the found variable space. How a slot finds a dynamic variable space is further explained on the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page. |
| `VariableExists` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Checks if the variable with the `VariableName` and with this component's sub type (the "<T>" of this component) exists in the found variable space. How a slot finds a dynamic variable space is further explained on the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page. |

Fields
Collapse

## Usage

## Examples

\- This component can be used to check if a battery is in a charger
\- This component can be used to control if functionality will work on an item.
\- This component can also be used for behavior of snappers or items by checking if the variable they are searching for exists or if the item is even connected to a space it can use.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicVariableStatus&oldid=93429](https://wiki.resonite.com/index.php?title=Component:DynamicVariableStatus&oldid=93429)"

Contents