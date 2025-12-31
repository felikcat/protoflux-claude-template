# Component:BoxMeshGizmo

> Source: https://wiki.resonite.com/Component:BoxMeshGizmo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BoxMeshGizmo&diff=92326) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dd/BoxMeshGizmoComponent.png/510px-BoxMeshGizmoComponent.png)](https://wiki.resonite.com/File:BoxMeshGizmoComponent.png) **Box Mesh Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BoxMeshGizmo** component is used to resize [Component:BoxMeshs](https://wiki.resonite.com/Component:BoxMesh "Component:BoxMesh") in a visual manner using the [DevTip](https://wiki.resonite.com/DevTip "DevTip").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [BoxMesh](https://wiki.resonite.com/Component:BoxMesh "Component:BoxMesh") >** | The box Mesh this component is targeting for editing. |
| `_cubeGizmo` | **[BoxGizmo](https://wiki.resonite.com/Component:BoxGizmo "Component:BoxGizmo")** | The visual for this component which is used to edit `_target` in a visual manner. |

Fields
Collapse

## Usage

Used to adjust the size of a box mesh. This can be accessed via the gizmo menu using a dev tip in your context menu. The button to activate it is the box mesh option.

## Examples

## See Also

- [DevTip](https://wiki.resonite.com/DevTip "DevTip")
- [Component:BoxColliderGizmo](https://wiki.resonite.com/Component:BoxColliderGizmo "Component:BoxColliderGizmo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxMeshGizmo&oldid=92326](https://wiki.resonite.com/index.php?title=Component:BoxMeshGizmo&oldid=92326)"

Contents