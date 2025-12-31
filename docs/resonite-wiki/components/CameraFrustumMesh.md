# Component:CameraFrustumMesh

> Source: https://wiki.resonite.com/Component:CameraFrustumMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CameraFrustumMesh&diff=97887) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7f/CameraFrustumMeshComponent.png/510px-CameraFrustumMeshComponent.png)](https://wiki.resonite.com/File:CameraFrustumMeshComponent.png) **Camera Frustum Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Camera Frustum Mesh is a component that can be used in a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to visualize the limits and view cone of a [Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")

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
| `Orientation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Direction the mesh is facing. |
| `Near` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Slices the mesh to demonstrate camera nearclip |
| `Far` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Expands the mesh to demonstrate camera farclip. |
| `HorizontalAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The horizontal FOV of the camera represented by this mesh. |
| `VerticalAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Vertical FOV of the camera represented by this mesh. |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enables the mesh to be dual sided. |
| `NearCap` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the end closest to the camera should be capped with a quad. |
| `FarCap` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the end furthest from the camera should be capped with a quad. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

The CameraFrustumMesh is used alongside the [InteractiveCamera](https://wiki.resonite.com/Component:InteractiveCamera "Component:InteractiveCamera") to visualize the range of the camera.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CameraFrustumMesh&oldid=97887](https://wiki.resonite.com/index.php?title=Component:CameraFrustumMesh&oldid=97887)"

Contents