# Component:ConstantCharacterControllerModifier

> Source: https://wiki.resonite.com/Component:ConstantCharacterControllerModifier

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5f/ConstantCharacterControllerModifierComponent.png/510px-ConstantCharacterControllerModifierComponent.png)](https://wiki.resonite.com/File:ConstantCharacterControllerModifierComponent.png) **Constant Character Controller Modifier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConstantCharacterController** component modifies the properties of a [Component:CharacterController](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") that makes contact with a character collider on the same Slot as this component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Parameter` | **[CharacterControllerParameter](https://wiki.resonite.com/Type:CharacterControllerParameter "Type:CharacterControllerParameter")** | The parameter to modify |
| `ModificationMode` | **[Mode](https://wiki.resonite.com/index.php?title=Type:Mode&action=edit&redlink=1 "Type:Mode (page does not exist)")** | How to modify the parameter. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the value to use in the modification. |

Fields
Collapse

## Usage

Attach to a slot with a collider that is a character collider. Then specify the settings this component should change and how. Then this component will be ready to use.

## Examples

Can be used to simulate sticky or slippery surfaces. Can also be used to simulate speedy gel from Portal2.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConstantCharacterControllerModifier&oldid=97285](https://wiki.resonite.com/index.php?title=Component:ConstantCharacterControllerModifier&oldid=97285)"

Contents