# Component:BallisticPathMesh

> Source: https://wiki.resonite.com/Component:BallisticPathMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BallisticPathMesh&diff=97868) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a0/BallisticPathMeshComponent.png/510px-BallisticPathMeshComponent.png)](https://wiki.resonite.com/File:BallisticPathMeshComponent.png) **Ballistic Path Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The ballistics path mesh is a component that generates a stripe or tube mesh that traces the future path of a virtual thrown object.

Tube mode currently does not work due to a small oversight. See [issue 2901](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/2901)

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
| `InitialPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The initial position of the ballistics path. |
| `InitialVelocity` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The initial velocity of the ballistics path. |
| `Gravity` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The gravity affecting the ballistics path (m/s^2) |
| `Drag` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the resistance through the air of the generated ballistics path |
| `Mode` | **[BallisticPathMesh.StepMode](https://wiki.resonite.com/Component:BallisticPathMesh#StepMode)** | What units `StepSize` is in. |
| `StepSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many units maximum every bend/segment is in length (the last segment may be shorter). |
| `TotalUnits` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many segments the path mesh will have give or take 1 or 2. |
| `Shape` | **[BallisticPathMesh.PathShape](https://wiki.resonite.com/Component:BallisticPathMesh#PathShape)** | What shape the arc should be rendered as. |
| `Size` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big to scale this ballisitics path |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many sides the tube mesh uses. Only accepts values greater than or equal to 3. |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the generated mesh should be dual sided. |
| `Up` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The up direction against gravity for the generated mesh (local space) |
| `DistanceSizeGrowth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to make the width/radius of the path mesh grow as it progresses along the arc. |
| `MinGrownSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How skinny at minimum the Ballistic Path Mesh will get from applying `DistanceSizeGrowth`. |
| `MaxGrownSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How wide at maximum the Ballistic Path Mesh will get from applying `DistanceSizeGrowth`. |
| `UseLastSegment` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to add one final segment that goes to <codr>LastSegmentPosition |
| `LastSegmentPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The local position to place the end of the last segment at if `UseLastSegment` is enabled. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## StepMode

| Name | Value | Description |
| --- | --- | --- |
| `Time` | 0 | `StepSize` refers to units of time |
| `Distance` | 1 | `StepSize` refers to distance in meters. |

Values

## PathShape

| Name | Value | Description |
| --- | --- | --- |
| `Stripe` | 0 | Make the path segment shape a sripe. |
| `Tube` | 1 | Make the path segment shape a tube. |

Values

## Usage

## Examples

This is commonly used in the teleport to locomotion for the indication visual for teleporting. The teleport locomotion uses Stripe for the path shape.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BallisticPathMesh&oldid=97868](https://wiki.resonite.com/index.php?title=Component:BallisticPathMesh&oldid=97868)"

Contents