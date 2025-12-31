# Component:MeshGizmo

> Source: https://wiki.resonite.com/Component:MeshGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/ce/MeshGizmoComponent.png/510px-MeshGizmoComponent.png)](https://wiki.resonite.com/File:MeshGizmoComponent.png) **Mesh Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Mesh Gizmo** component is used to set up and generate the visuals/behavior of mesh orbs which are physical item/references to mesh data.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [StaticMesh](https://wiki.resonite.com/Component:StaticMesh "Component:StaticMesh") >** | The static mesh that this is referencing and displaying. |
| `_inspectorRoot` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The inspector this component generated when it was made. |

Fields
Collapse

## Usage

Used in mesh orbs used with the [Mesh Tool](https://wiki.resonite.com/Mesh_Tool "Mesh Tool") and with scene inspectors for allowing physical hold able access to meshes for use in static and skinned mesh renderers.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

We need images here.

## See Also

- [Mesh Tool](https://wiki.resonite.com/Mesh_Tool "Mesh Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshGizmo&oldid=105328](https://wiki.resonite.com/index.php?title=Component:MeshGizmo&oldid=105328)"

Contents