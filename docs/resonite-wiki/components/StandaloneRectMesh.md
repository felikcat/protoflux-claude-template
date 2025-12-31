# Component:StandaloneRectMesh

> Source: https://wiki.resonite.com/Component:StandaloneRectMesh

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ad/StandaloneRectMesh%601Component.png/510px-StandaloneRectMesh%601Component.png)](https://wiki.resonite.com/File:StandaloneRectMesh%601Component.png) **Standalone Rect Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StandaloneRectMesh** is a procedural wrapper to allow mesh renderer usable mesh data of any [RectMeshSource](https://wiki.resonite.com/Type:RectMeshSource "Type:RectMeshSource"). The list of [RectMeshSources](https://wiki.resonite.com/Type:RectMeshSource "Type:RectMeshSource") this component can use for **M** is generated inside the component selector list when attaching.

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
| `Rect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The part of the generated waveform to render. |
| `Mesh` | _direct_ **M** | The mesh parameters used to render this rect mesh. Usually takes an audio clip. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

[ProbablePrime's](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime") video tutorial on how to use this component:

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- Similar to [RectMesh](https://wiki.resonite.com/Component:RectMesh "Component:RectMesh").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StandaloneRectMesh&oldid=98076](https://wiki.resonite.com/index.php?title=Component:StandaloneRectMesh&oldid=98076)"

Contents