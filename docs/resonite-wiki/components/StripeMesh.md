# Component:StripeMesh

> Source: https://wiki.resonite.com/Component:StripeMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StripeMesh&diff=98084) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/78/StripeMeshComponent.png/510px-StripeMeshComponent.png)](https://wiki.resonite.com/File:StripeMeshComponent.png) **Stripe Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StripeMesh** component generates mesh data that is used with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

_This article or section is a stub. You can help the Resonite wiki by expanding it._

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
| `Points` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[StripePoint](https://wiki.resonite.com/index.php?title=Type:StripePoint&action=edit&redlink=1 "Type:StripePoint (page does not exist)")** | The points used to generate the geometry for this mesh. |
| `SegmentPoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many cuts/bends are between each point. Higher means more detail |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this mesh is visible from the back and front. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach this component to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the geometry. Don't forget to add a [Material](https://wiki.resonite.com/Material "Material").

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StripeMesh&oldid=98084](https://wiki.resonite.com/index.php?title=Component:StripeMesh&oldid=98084)"

Contents