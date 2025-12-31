# Component:BevelPlaneMesh

> Source: https://wiki.resonite.com/Component:BevelPlaneMesh

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6f/BevelPlaneMeshComponent.png/510px-BevelPlaneMeshComponent.png)](https://wiki.resonite.com/File:BevelPlaneMeshComponent.png) **Bevel Plane Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Used in old Legacy content like old inspectors and panels.

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
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the width of the plane |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the height of the plane |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How 3D the plane should be, making it more like a box. |
| `TopLeftCut` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to bevel the top left corner. |
| `BottomRightCut` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to bevel the bottom right corner. |
| `Relief` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | indent the center inwards or not. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot, and use the `Settup Renderer` button to view the mesh.

## Examples

Used in old legacy UI from [migrated](https://wiki.resonite.com/Migrations "Migrations") content.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BevelPlaneMesh&oldid=97871](https://wiki.resonite.com/index.php?title=Component:BevelPlaneMesh&oldid=97871)"

Contents