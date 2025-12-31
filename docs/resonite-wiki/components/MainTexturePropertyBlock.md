# Component:MainTexturePropertyBlock

> Source: https://wiki.resonite.com/Component:MainTexturePropertyBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MainTexturePropertyBlock&diff=89106) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/62/MainTexturePropertyBlockComponent.png/510px-MainTexturePropertyBlockComponent.png)](https://wiki.resonite.com/File:MainTexturePropertyBlockComponent.png) **Main Texture Property Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MainTexturePropertyBlock** component is a [Material Property Block](https://wiki.resonite.com/Material_Property_Block "Material Property Block") for the main texture of a component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | Texture to swap out the main texture with. |

Fields
Collapse

## Usage

This component allows one to swap out what a material considers its main texture, such as the albedo texture, with the given `Texture`. This property block only applies to materials that contain a `_MainTex` material property field. Notably, [UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial") does not support this property block.

## Examples

A good use for this component could be a picture wall, wherein a significant amount of pictures that should look the same but with different textures can be built with efficient memory usage and initial draw calls. Each picture would have its own [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") using the same material but with its own MainTexturePropertyBlock.

## See Also

- [Material Property Block](https://wiki.resonite.com/Material_Property_Block "Material Property Block")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MainTexturePropertyBlock&oldid=89106](https://wiki.resonite.com/index.php?title=Component:MainTexturePropertyBlock&oldid=89106)"

Contents