# Component:ColorWheelTriangleMesh

> Source: https://wiki.resonite.com/Component:ColorWheelTriangleMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4e/ColorWheelTriangleMeshComponent.png/510px-ColorWheelTriangleMeshComponent.png)](https://wiki.resonite.com/File:ColorWheelTriangleMeshComponent.png) **Color Wheel Triangle Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorWheelTriangleMesh** component is used in the old platform's color pickers. Some may call this a "flower" or a "color picker" visual.

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
| `Hue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Hue the user picked. |
| `OuterRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the outer edge of the outer ring of the color circle of hues. |
| `InnerRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the inner edge of the outer ring of the color circle of hues. |
| `RingSegments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many ring wise subdivisions of the outer ring of color hues. |
| `CursorPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the cursor inside of the triangle. |
| `CursorSegments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many ring wise subdivisions of the color picker cursor ring. |
| `CursorColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the cursor for color picking. |
| `CursorOuterRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the outer edge of the cursor ring. |
| `CursorInnerRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the inner edge of the cursor ring. |
| `CursorZOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the color picker cursor off the surface of the triangle. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") that supports vertex colors to view what it looks like.

## Examples

Used in color pickers from other platform content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorWheelTriangleMesh&oldid=97898](https://wiki.resonite.com/index.php?title=Component:ColorWheelTriangleMesh&oldid=97898)"

Contents