# Component:EyeRotationDriverGizmo

> Source: https://wiki.resonite.com/Component:EyeRotationDriverGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fd/EyeRotationDriverGizmoComponent.png/510px-EyeRotationDriverGizmoComponent.png)](https://wiki.resonite.com/File:EyeRotationDriverGizmoComponent.png) **Eye Rotation Driver Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **EyeRotationDriverGizmo** component is used to edit the Eye forwards of an [Eye Rotation Driver](https://wiki.resonite.com/Component:EyeRotationDriver "Component:EyeRotationDriver").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [EyeRotationDriver](https://wiki.resonite.com/Component:EyeRotationDriver "Component:EyeRotationDriver") >** | The eye rotation driver we are editing. |
| `_vectorGizmos` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[VectorGizmo](https://wiki.resonite.com/Component:VectorGizmo "Component:VectorGizmo")** | The forward vectors of the eyes. |
| `_coneGizmos` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[ConeGizmo](https://wiki.resonite.com/Component:ConeGizmo "Component:ConeGizmo")** | Unused. Possibly a bug. |

Fields
Collapse

## Usage

Found in the [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool") gizmo menu when selecting a slot with a [Component:EyeRotationDriver](https://wiki.resonite.com/Component:EyeRotationDriver "Component:EyeRotationDriver") on it.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:EyeRotationDriver](https://wiki.resonite.com/Component:EyeRotationDriver "Component:EyeRotationDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EyeRotationDriverGizmo&oldid=96457](https://wiki.resonite.com/index.php?title=Component:EyeRotationDriverGizmo&oldid=96457)"

Contents