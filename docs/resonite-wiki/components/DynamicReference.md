# Component:DynamicReference

> Source: https://wiki.resonite.com/Component:DynamicReference

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicReference&diff=97317) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1c/DynamicReference%601Component.png/510px-DynamicReference%601Component.png)](https://wiki.resonite.com/File:DynamicReference%601Component.png) **Dynamic Reference\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicReference** component allows marking of any [SyncRef\`1 (Reference holder)](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") as part of the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. The value inside of the specified [SyncRef](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") can change and will be changed by the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. The variable name and the type of variable will determine how this will link to and be changed by the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. For more info on how Dynamic Variables work please check the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Variable name that will be used to link this component's refrenced value to the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. |
| `TargetReference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>>** | The field to become synced with and be the definition of the reference dynamic variable. |
| `OverrideOnLink` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether this component should write its value to a [Dynamic Variable Space Component](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") when it links to the space, updating all child variables with the same name and type. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicReference&oldid=97317](https://wiki.resonite.com/index.php?title=Component:DynamicReference&oldid=97317)"

Contents