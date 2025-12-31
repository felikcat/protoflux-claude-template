# Component:Projection360PropertyBlock

> Source: https://wiki.resonite.com/Component:Projection360PropertyBlock

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Projection360PropertyBlock&diff=91418) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/18/Projection360PropertyBlockComponent.png/510px-Projection360PropertyBlockComponent.png)](https://wiki.resonite.com/File:Projection360PropertyBlockComponent.png) **Projection360 Property Block** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Material Property Block](https://wiki.resonite.com/Material_Property_Block "Material Property Block") for a vastly detailed explaination.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to override the `Texture` field of a [Projection360Material](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material") for a renderer. |
| `PerspectiveFieldOfView` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The value to override the `PerspectiveFieldOfView` field of a [Projection360Material](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material") for a renderer. |
| `PerspectiveAngleOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The value to override the `PerspectiveAngleOffset` field of a [Projection360Material](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material") for a renderer. |

Fields
Collapse

## Usage

See [Material Property Block](https://wiki.resonite.com/Material_Property_Block "Material Property Block") for a vastly detailed explaination.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Projection360PropertyBlock&oldid=91418](https://wiki.resonite.com/index.php?title=Component:Projection360PropertyBlock&oldid=91418)"

Contents