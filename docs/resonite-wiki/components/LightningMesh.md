# Component:LightningMesh

> Source: https://wiki.resonite.com/Component:LightningMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LightningMesh&diff=98659) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4e/LightningMeshComponent.png/510px-LightningMeshComponent.png)](https://wiki.resonite.com/File:LightningMeshComponent.png) **Lightning Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LightingMesh** component generates geometry of a procedural lighting bolt for use with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

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
| `Seed` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Used to generate a pseudo-random variant of a lighting bolt mesh |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how much detail the lighting bolt should have. |
| `Topology` | **[Topology](https://wiki.resonite.com/index.php?title=Type:Topology&action=edit&redlink=1 "Type:Topology (page does not exist)")** | The Topology setting for the lighting bolt |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | The shading for the lighting bolt geometry. Like smooth or flat for example. |
| `Ends` | **[Ends](https://wiki.resonite.com/Type:Ends "Type:Ends")** | how to handle the geometry at the beginning and end of lines in the lighting bolt |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the lighting bolt is visible from the inside. |
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the start point of the lightning bolt |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the end point of the lightning bolt |
| `StrikeLevels` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LightningMesh.StrikeProperties](https://wiki.resonite.com/Component:LightningMesh#StrikeProperties)** | A list of different branch variants and bends in the lighting bolt. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the geometry it generates. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## StrikeProperties

Generates a group of lines that shoot out at random bent angles with multiple segments. The start and end of these forks in the lighting mesh can be controlled via its settings.

| Name | Type | Description |
| --- | --- | --- |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The detail of this fork group |
| `StartWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the width of the start of the forks of this fork segment. |
| `EndWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the width of the end of the forks of this fork segment. |
| `MinOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum offset from the start of the lighting bolt for this fork group |
| `MaxOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum offset from the start of the lighting bolt for this fork group |
| `ChildCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of forks in this fork group |
| `MinChildTargetDistanceRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum distance of the children of this fork group from the center bolt. |
| `MaxChildTargetDistanceRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum distance of the children of the fork group from the center bolt. |
| `MinChildTargetOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum target offset for children of this fork group. |
| `MaxChildTargetOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum target offset for children of this fork group. |

Fields

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LightningMesh&oldid=98659](https://wiki.resonite.com/index.php?title=Component:LightningMesh&oldid=98659)"

Contents