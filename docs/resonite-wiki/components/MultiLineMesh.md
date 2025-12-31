# Component:MultiLineMesh

> Source: https://wiki.resonite.com/Component:MultiLineMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MultiLineMesh&diff=98004) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bd/MultiLineMeshComponent.png/510px-MultiLineMeshComponent.png)](https://wiki.resonite.com/File:MultiLineMeshComponent.png) **Multi Line Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MultiLineMesh** component generates geometry for use with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"). For now, this component is unusable without [Mods](https://wiki.resonite.com/Mods "Mods") due to having a list type object.

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
| `Lines` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[MultiLineMesh.Line](https://wiki.resonite.com/Component:MultiLineMesh#Line)** | A set of lines that make up the source of the data for the geometry of this mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Line

| Name | Type | Description |
| --- | --- | --- |
| `Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the line. This is a multiplier. |
| `Color` | **[Color](https://wiki.resonite.com/Type:Color "Type:Color")** | The vertex color of the line |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many points are in this line. |
| `Topology` | **[Topology](https://wiki.resonite.com/index.php?title=Type:Topology&action=edit&redlink=1 "Type:Topology (page does not exist)")** | the kind of Topology this line has. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | How to handle the Shading of this line. |
| `Ends` | **[Ends](https://wiki.resonite.com/Type:Ends "Type:Ends")** | How to handle the caps at the start and end of this line |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the line can be seen from the inside. |
| `AbsolutePointOffets` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether each position is relative or not from the last point |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale of the material detail on the surface of this line. |
| `ScaleUVByCircumference` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to keep the material detail per square millimeter consistent regardless of the value used for `Scale` |
| `PreciseUV` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make a more accurate UV for the line. |
| `Positions` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A list of positions to use for making the line |
| `Scales` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scale of each line segment. Each one is multipled by `Scales` for the final geometry. |
| `Orientations` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of each segment of the line |
| `Colors` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Color](https://wiki.resonite.com/Type:Color "Type:Color")** | The vertex colors of each segment of the line |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile used for the vertex colors of this line. |
| `PointOffsets` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of each point of the line. Used in tandem with `Orientations` to handle line shape. |

Fields

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the generated geometry. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiLineMesh&oldid=98004](https://wiki.resonite.com/index.php?title=Component:MultiLineMesh&oldid=98004)"

Contents