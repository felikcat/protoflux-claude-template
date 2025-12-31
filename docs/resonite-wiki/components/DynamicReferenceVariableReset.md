# Component:DynamicReferenceVariableReset

> Source: https://wiki.resonite.com/Component:DynamicReferenceVariableReset

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicReferenceVariableReset&diff=80403) which are not marked for translation.

Dynamic Reference Variable Reset is a component that will reset the value for a [Dynamic Variable](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") to a specified Reference. This is useful for when you are messing with an item, but you want the values for it to clear themselves with it is saved, loaded, or duplicated. The variable space is determined by the searching algorithm explained on [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page from the slot this is on.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c4/DynamicReferenceVariableReset%601Component.png/510px-DynamicReferenceVariableReset%601Component.png)](https://wiki.resonite.com/File:DynamicReferenceVariableReset%601Component.png) **Dynamic Reference Variable Reset\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Variable name that will be used to link this component's refrenced value to the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") System. |
| `ResetOnLoad` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reset when this component is loaded with a world. |
| `ResetOnDuplicate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reset when the object this is under is duplicated. |
| `ResetOnPaste` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Reset when the object this is under is pasted from clipboard. |
| `ResetTarget` | **T** | The reference value to reset to when any of the enabled reset events occur. |

Fields
Collapse

## Usage

## Examples

If you use this component with a slot selector, you can make the selection go null when the object is loaded or loaded with a world. This can be useful for something like a teleporter system or something, where you want the user to select where they want to go when the world loads, rather than being left at the last value it was at when the world was saved.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicReferenceVariableReset&oldid=80403](https://wiki.resonite.com/index.php?title=Component:DynamicReferenceVariableReset&oldid=80403)"

Contents