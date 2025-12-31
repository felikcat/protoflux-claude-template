# Component:DynamicReferenceVariableDriver

> Source: https://wiki.resonite.com/Component:DynamicReferenceVariableDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicReferenceVariableDriver&diff=97315) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5f/DynamicReferenceVariableDriver%601Component.png/510px-DynamicReferenceVariableDriver%601Component.png)](https://wiki.resonite.com/File:DynamicReferenceVariableDriver%601Component.png) **Dynamic Reference Variable Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicReferenceVariableDriver** component can drive a [SyncRef\`1 (Reference Holder)](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") to the value assigned to a dynamic variable with the name `VariableName`. if the specified variable cannot be found, the value will revert to `DefaultTarget` how this works is explained on [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Variable name that will be used to link this component's refrenced value to the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. |
| `Target` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | The field to drive with the variable definition. |
| `DefaultTarget` | **T** | The value/reference to revert to when this component cannot find the specified `VariableName` dynamic variable. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

This component can be used as a way of abusing how dynamic variables are read by making this component with a [slot type](https://wiki.resonite.com/Type:Slot "Type:Slot"). Since this component reads from the slot it is on, this component can drive the parent field of another slot. Using this in tandem allows for interesting behavior.
For example:
Start with an avatar that has a slot on it's head, with a [DynamicReferenceVariable<Slot>](https://wiki.resonite.com/Component:DynamicReferenceVariable "Component:DynamicReferenceVariable") pointing to it with the `VariableName` field having "User/Hat" in it. then have an item like a hat stand with the stand slot having a DynamicReferenceVariableDriver< [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") \> with a `VariableName` with "User/Hat" on it. the `DefaultTarget` would be the slot the component is on, which is the hat stand. The hat stand would a hat parented to it. the hat would have it's parent field driven by the component on the hat stand. Since the hat stand would be sitting in a world, the hat will stay on the stand, since it can't find the variable, "User/Hat". the second a user picks the stand up with a slot variable that is named "User/Hat", the hat will move from the stand to the slot specified by the variable on that user. Keep in mind, that the hat in this scenario has nothing to do with how the variable is read, but rather the stand does. When the stand unparents from the user, the slot sampling the variable space which is the stand can no longer find the variable. What then happens is the field the DynamicReferenceVariableDriver< [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") \> is driving will revert to `DefaultTarget` which is the stand slot, making it move back to the stand.

This also allows for the slot that moves (also known as the hat) to sample values too, allowing for even more complex reading and interaction (EX: the hat moves to the user's head and changes color to the user's color)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicReferenceVariableDriver&oldid=97315](https://wiki.resonite.com/index.php?title=Component:DynamicReferenceVariableDriver&oldid=97315)"

Contents