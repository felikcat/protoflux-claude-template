# Component:TextureCharacterControllerModifier

> Source: https://wiki.resonite.com/Component:TextureCharacterControllerModifier

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1f/TextureCharacterControllerModifierComponent.png/510px-TextureCharacterControllerModifierComponent.png)](https://wiki.resonite.com/File:TextureCharacterControllerModifierComponent.png) **Texture Character Controller Modifier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureCharacterControllerModifier** component reacts to [character controllers](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") that collide with [mesh colliders](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider") in its children hiearchy. It starts by finding what the contact triangle and point on the [mesh collider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider") a [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") hit was. That point is mapped to what part of a texture the [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") hit. Finally, the texture data in `Texture` is used to determine what the value should be used for Modifying the [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") that hit that [mesh collider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Parameter` | **[CharacterControllerParameter](https://wiki.resonite.com/Type:CharacterControllerParameter "Type:CharacterControllerParameter")** | The parameter of the contacting [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") to modify. |
| `ModificationMode` | **[Mode](https://wiki.resonite.com/index.php?title=Type:Mode&action=edit&redlink=1 "Type:Mode (page does not exist)")** | How to modify the parameter on the contacting [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController"). |
| `MinValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When the mapped value on `Texture` maps to a value of 0, what should the value be for the [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") modification? |
| `MaxValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When the mapped value on `Texture` maps to a value of 100% brightness or 1, what should the value be for the [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") modification? |
| `Channel` | **[ColorChannel](https://wiki.resonite.com/index.php?title=Type:ColorChannel&action=edit&redlink=1 "Type:ColorChannel (page does not exist)")** | The channel to use on `Texture` when getting a value for UV contact points. |
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to use for character controller modification data. |

Fields
Collapse

## Usage

Attach to the same slot as a mesh collider for best results. A packed texture of RBGA can be used and reused for this component to save on resources and modify 4 different values on 4 different instances of this component to allow for Modifying 4 different character controller properties at the same time.

## Examples

Can be used as the character physics equivalent of a [color splat map material](https://wiki.resonite.com/Color_Splat_Materials "Color Splat Materials") to allow different terrain like sand or gravel to affect user speed or jump height when walking on it.
This can also be used to make a golf course, where the simulated ball can be affected by sand pits or goo.

## See Also

- [Color Splat Materials](https://wiki.resonite.com/Color_Splat_Materials "Color Splat Materials") to create terrain that acts as the visuals for the physical effects of this component.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureCharacterControllerModifier&oldid=97778](https://wiki.resonite.com/index.php?title=Component:TextureCharacterControllerModifier&oldid=97778)"

Contents