# Component:DynamicValueVariable

> Source: https://wiki.resonite.com/Component:DynamicValueVariable

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicValueVariable&diff=97319) which are not marked for translation.

A dynamic value variable is a component that allows storing any value [Type](https://wiki.resonite.com/Category:Type "Category:Type") inside the component. The value is then accessible and changeable via the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") system.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6a/DynamicValueVariable%601Component.png/510px-DynamicValueVariable%601Component.png)](https://wiki.resonite.com/File:DynamicValueVariable%601Component.png) **Dynamic Value Variable\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Variable name that will be used to link this component's refrenced value to the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. |
| `Value` | **T** | The value this variable holds. Can set and be changed by the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") system. |
| `OverrideOnLink` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether this component should write its value to a [Dynamic Variable Space Component](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") when it links to the space, updating all child variables with the same name and type. |

Fields
Collapse

## Usage

This can be used to store values that should be accessible to different things underneath and outside of a system. This is useful if the item needs to be able to have it's color changed, or other properties that need to have quick synchronization and access. For more info see the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicValueVariable&oldid=97319](https://wiki.resonite.com/index.php?title=Component:DynamicValueVariable&oldid=97319)"

Contents