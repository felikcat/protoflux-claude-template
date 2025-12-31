# Component:SubmeshCharacterControllerModifier

> Source: https://wiki.resonite.com/Component:SubmeshCharacterControllerModifier

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fc/SubmeshCharacterControllerModifierComponent.png/510px-SubmeshCharacterControllerModifierComponent.png)](https://wiki.resonite.com/File:SubmeshCharacterControllerModifierComponent.png) **Submesh Character Controller Modifier** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SubmeshCharacterController** is a component able to change properties of a [Person or NPC locomotion (Character Controller)](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") walking on a mesh based on what submesh of the mesh they are walking on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Parameter` | **[CharacterControllerParameter](https://wiki.resonite.com/Type:CharacterControllerParameter "Type:CharacterControllerParameter")** | The parameter to modify |
| `ModificationMode` | **[Mode](https://wiki.resonite.com/index.php?title=Type:Mode&action=edit&redlink=1 "Type:Mode (page does not exist)")** | How to modify the parameter. |
| `Values` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | What value to use when modifying for each sub mesh. In order of submesh number. |

Fields
Collapse

## Usage

Attach to the same slot as a mesh collider with a mesh set to static and IsCharacterCollider in order for this to work.

## Examples

Can be used to make a checkered floor that has sticky or slidy tiles depending on what a user steps on within one mesh if the submeshes are set up correctly.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SubmeshCharacterControllerModifier&oldid=97770](https://wiki.resonite.com/index.php?title=Component:SubmeshCharacterControllerModifier&oldid=97770)"

Contents