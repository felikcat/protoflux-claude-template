# Component:TubeMesh

> Source: https://wiki.resonite.com/Component:TubeMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TubeMesh&diff=98100) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/95/TubeMeshComponent.png/510px-TubeMeshComponent.png)](https://wiki.resonite.com/File:TubeMeshComponent.png) **Tube Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TubeMesh** component is used to generate a procedural tube mesh for use with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

The `Points` field currently requires [Mods](https://wiki.resonite.com/Mods "Mods") to edit.

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
| `Points` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[TubePoint](https://wiki.resonite.com/index.php?title=Type:TubePoint&action=edit&redlink=1 "Type:TubePoint (page does not exist)")** | A list of points that the tube should follow in order. |
| `SegmentPoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many cuts/bend points there should be between each [TubePoint](https://wiki.resonite.com/index.php?title=Type:TubePoint&action=edit&redlink=1 "Type:TubePoint (page does not exist)") in `Points` |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach the component into a slot and insert it into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the geometry. Don't forget a [Material](https://wiki.resonite.com/Material "Material").

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TubeMesh&oldid=98100](https://wiki.resonite.com/index.php?title=Component:TubeMesh&oldid=98100)"

Contents