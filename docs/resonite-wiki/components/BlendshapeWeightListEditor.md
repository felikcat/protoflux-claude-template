# Component:BlendshapeWeightListEditor

> Source: https://wiki.resonite.com/Component:BlendshapeWeightListEditor

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BlendshapeWeightListEditor&diff=91236) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6a/BlendshapeWeightListEditorComponent.png/510px-BlendshapeWeightListEditorComponent.png)](https://wiki.resonite.com/File:BlendshapeWeightListEditorComponent.png) **Blendshape Weight List Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Weight list editor is a component that is used within inspectors and shouldn't need to be interacted with by the user. Although, it can be used in very niche circumstances.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetList` | **[ISyncList](https://wiki.resonite.com/Type:ISyncList "Type:ISyncList")** | The list of blendshapes. This can be acquired through grabbing the "BlendShapes" title at the beginning of a blendshape list inside of a [Skinned Mesh Renderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") |
| `_addNewButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that when pressed, should add a new blendshape to the end of the `_targetList`. Whether the new blendshape does anything or not depends on if the `Mesh` data inside of `_targetSkin` has a blendshape list that reaches as far as the new item. |
| `_targetSkin` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") >** | The skinned Mesh renderer to add a new blendshape item to. Has to be the same component `_targetList` comes from. |

Fields
Collapse

## Usage

Add component to a slot and fill the fields, with the proper data explained in the table above. Press the button provided to `_addNewButton` to add a new blendshape to the targeted skinned Mesh renderer.

## Examples

Generated automatically inside of inspectors to allow the modification of blendshape lists.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BlendshapeWeightListEditor&oldid=91236](https://wiki.resonite.com/index.php?title=Component:BlendshapeWeightListEditor&oldid=91236)"

Contents