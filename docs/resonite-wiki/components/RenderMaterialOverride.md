# Component:RenderMaterialOverride

> Source: https://wiki.resonite.com/Component:RenderMaterialOverride

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/65/RenderMaterialOverrideComponent.png/510px-RenderMaterialOverrideComponent.png)](https://wiki.resonite.com/File:RenderMaterialOverrideComponent.png) **Render Material Override** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RenderMaterialOverride** Component allows for overriding materials on a renderer when it is rendered in certain contexts.

Note: This only overrides materials properly if all `Context`s are used, with a component for each one. This may be a bug.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Context` | **[RenderingContext](https://wiki.resonite.com/Type:RenderingContext "Type:RenderingContext")** | The context in which to override the materials of `Renderer` with the list of `Overrides`. |
| `Renderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The renderer to override materials for. |
| `Overrides` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[RenderMaterialOverride.MaterialOverride](https://wiki.resonite.com/Component:RenderMaterialOverride#MaterialOverride)** | A list of materials to override during rendering in a `Context` context. |

Fields
Collapse

## MaterialOverride

| Name | Type | Description |
| --- | --- | --- |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The material index on `Renderer` to override. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to override `Renderer`'s materials for material `Index`. |

Fields

## Usage

Used to hide materials or change them in a mirror. like showing an evil version of yourself in a mirror, or to hide your head material from your own viewpoint

## Examples

## See Also

- [Component:RenderTransformOverride](https://wiki.resonite.com/Component:RenderTransformOverride "Component:RenderTransformOverride")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RenderMaterialOverride&oldid=97707](https://wiki.resonite.com/index.php?title=Component:RenderMaterialOverride&oldid=97707)"

Contents