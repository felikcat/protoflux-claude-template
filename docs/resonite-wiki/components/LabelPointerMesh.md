# Component:LabelPointerMesh

> Source: https://wiki.resonite.com/Component:LabelPointerMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LabelPointerMesh&diff=97971) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6a/LabelPointerMeshComponent.png/510px-LabelPointerMeshComponent.png)](https://wiki.resonite.com/File:LabelPointerMeshComponent.png) **Label Pointer Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LabelPointerMesh** component is used by the labeler tool to point to a position and underline some generated text elements.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `LabelPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Where the label should render in local space. |
| `TargetPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Where the line from the label should point to. |
| `LabelRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the label visual. |
| `LabelWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the label visual. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the line going from the label to `TargetPoint` |
| `ExpandLerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the label underline should be. |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the mesh should have duplicate geometry with the fronts facing the opposite direction. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Examples

Used by the labeler tool.

## See Also

- [Labeler Tool](https://wiki.resonite.com/Labeler_Tool "Labeler Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LabelPointerMesh&oldid=97971](https://wiki.resonite.com/index.php?title=Component:LabelPointerMesh&oldid=97971)"

Contents