# Component:MultiBevelStripeMesh

> Source: https://wiki.resonite.com/Component:MultiBevelStripeMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/03/MultiBevelStripeMeshComponent.png/510px-MultiBevelStripeMeshComponent.png)](https://wiki.resonite.com/File:MultiBevelStripeMeshComponent.png) **Multi Bevel Stripe Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MultiBevelStripeMesh** component can be used to instanciate multiple [Component:BevelStripeMeshs](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh") as part of the same geometry.

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
| `Stripes` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[MultiBevelStripeMesh.Stripe](https://wiki.resonite.com/Component:MultiBevelStripeMesh#Stripe)** | A list of stripes to render. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Stripe

Stripe represents the exact values in a [Component:BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh") with an added position, rotation, and scale settings.

| Name | Type | Description |
| --- | --- | --- |
| `Position_Field` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the Bevel Stripe mesh. |
| `Rotation_Field` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the Bevel Stripe mesh. |
| `Scale_Field` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of the Bevel Stripe mesh. |
| `Width_Field` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the cube |
| `Height_Field` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the height of the cube |
| `Thickness_Field` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the length of the cube. |
| `SlantLeft_Field` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the Bevel angle of the length wise edge on the top left. |
| `SlantRight_Field` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the Bevel angle of the length wise edge on the bottom right. |
| `Relief_Field` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to indent the cube in the center. |

Fields

## Usage

Can be used to instanciate many Bevel Stripe meshes at once for organization and performance improvement.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiBevelStripeMesh&oldid=98003](https://wiki.resonite.com/index.php?title=Component:MultiBevelStripeMesh&oldid=98003)"

Contents