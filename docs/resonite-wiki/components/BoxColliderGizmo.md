# Component:BoxColliderGizmo

> Source: https://wiki.resonite.com/Component:BoxColliderGizmo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BoxColliderGizmo&diff=93415) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/42/BoxColliderGizmoComponent.png/510px-BoxColliderGizmoComponent.png)](https://wiki.resonite.com/File:BoxColliderGizmoComponent.png) **Box Collider Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BoxColliderGizmo** component is used to resize and move [Component:BoxColliders](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider") in a visual manner using the [DevTip](https://wiki.resonite.com/DevTip "DevTip").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider") >** | The box collider this component is currently editing |
| `_cubeGizmo` | **[BoxGizmo](https://wiki.resonite.com/Component:BoxGizmo "Component:BoxGizmo")** | The visual for this component which is used to edit `_target` in a visual manner. |

Fields
Collapse

## Usage

Used to adjust the size of a box collider. This can be accessed via the gizmo menu using a dev tip in your context menu. The button to activate it is the box collider option.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [DevTip](https://wiki.resonite.com/DevTip "DevTip")
- [Component:BoxMeshGizmo](https://wiki.resonite.com/Component:BoxMeshGizmo "Component:BoxMeshGizmo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxColliderGizmo&oldid=93415](https://wiki.resonite.com/index.php?title=Component:BoxColliderGizmo&oldid=93415)"

Contents