# Component:MainAndMaskTexturePropertyBlock

> Source: https://wiki.resonite.com/Component:MainAndMaskTexturePropertyBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MainAndMaskTexturePropertyBlock&diff=94891) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/02/MainAndMaskTexturePropertyBlockComponent.png/510px-MainAndMaskTexturePropertyBlockComponent.png)](https://wiki.resonite.com/File:MainAndMaskTexturePropertyBlockComponent.png) **Main And Mask Texture Property Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MainAndMaskTexturePropertyBlock** component is used to modify material properties on [mesh renderers](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") and [skinned mesh renderers](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") as part of their material Property blocks. This is useful in instances where having lots of extra materials is less performant than modifying a material using a Property Block.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to replace the Main texture on a material with. |
| `MaskTexture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to replace the Mask texture on a material with. |

Fields
Collapse

## Usage

Can be used to optimize many materials that only differ in main and mask texture properties.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MainAndMaskTexturePropertyBlock&oldid=94891](https://wiki.resonite.com/index.php?title=Component:MainAndMaskTexturePropertyBlock&oldid=94891)"

Contents