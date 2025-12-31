# Component:ColorDepthGrid

> Source: https://wiki.resonite.com/Component:ColorDepthGrid

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5b/ColorDepthGridComponent.png/510px-ColorDepthGridComponent.png)](https://wiki.resonite.com/File:ColorDepthGridComponent.png) **Color Depth Grid** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `ColorTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** |  |
| `DepthTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** |  |
| `Projection` | **[PointProjection](https://wiki.resonite.com/Type:PointProjection "Type:PointProjection")** |  |
| `HorizontalAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `VerticalAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `DepthOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `DepthScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Behavior

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorDepthGrid&oldid=97893](https://wiki.resonite.com/index.php?title=Component:ColorDepthGrid&oldid=97893)"

Contents