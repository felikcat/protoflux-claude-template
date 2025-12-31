# Component:DynamicValueVariableReset

> Source: https://wiki.resonite.com/Component:DynamicValueVariableReset

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicValueVariableReset&diff=80406) which are not marked for translation.

Dynamic Value Variable Reset is a component that will reset the value for a [Dynamic Variable](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") to a specified Value. This is useful for when you are messing with an item, but you want the values for it to clear themselves with it is saved, loaded, or duplicated. The variable space is determined by the searching algorithm explained on [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page from the slot this is on.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/37/DynamicValueVariableReset%601Component.png/510px-DynamicValueVariableReset%601Component.png)](https://wiki.resonite.com/File:DynamicValueVariableReset%601Component.png) **Dynamic Value Variable Reset\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

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
| `ResetValue` | **T** | The value to reset to when any of the enabled reset events occur. |

Fields
Collapse

## Usage

## Examples

\- [989onan's](https://wiki.resonite.com/User:989onan "User:989onan") cloud home uses this for their multi personality room in their cloud home. When they load in the world, this component has `ResetOnLoad` enabled to reset an [int](https://wiki.resonite.com/Type:Int "Type:Int") on a multiplexer that determines which room is visible to 0. That way if another personality saves the world to save their room changes, the component will reset the index to a blank room, so other personalities don't snoop onto someone else's belongings.

\- A selection of a song on a menu can be changed with this, by making the selection part of a [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") system.

\- Settings like checkmarks can be reset when the item is saved by another player, so the item doesn't need [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to handle such cases.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicValueVariableReset&oldid=80406](https://wiki.resonite.com/index.php?title=Component:DynamicValueVariableReset&oldid=80406)"

Contents