# Component:DebugTestMeshThroughput

> Source: https://wiki.resonite.com/Component:DebugTestMeshThroughput

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0f/DebugTestMeshThroughputComponent.png/510px-DebugTestMeshThroughputComponent.png)](https://wiki.resonite.com/File:DebugTestMeshThroughputComponent.png) **Debug Test Mesh Throughput** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugTestMeshThroughput** component is used in code by parallel jamming quads into a MeshX object via multithreading to test how much can be done at once.

The mesh generated is a Spiral fan of quads that goes up in a circle pattern.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


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
| `Count` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many mesh quads to parrallel jam into the meshx data. |
| `Progress` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the quads by in rotation. |
| `UpdateTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long it took for the Asset to update. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Debugging MeshX parallel speed.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugTestMeshThroughput&oldid=97917](https://wiki.resonite.com/index.php?title=Component:DebugTestMeshThroughput&oldid=97917)"

Contents