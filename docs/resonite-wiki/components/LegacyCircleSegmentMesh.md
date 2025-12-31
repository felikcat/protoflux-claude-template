# Component:LegacyCircleSegmentMesh

> Source: https://wiki.resonite.com/Component:LegacyCircleSegmentMesh

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/LegacyCircleSegmentMeshComponent.png/510px-LegacyCircleSegmentMeshComponent.png)](https://wiki.resonite.com/File:LegacyCircleSegmentMeshComponent.png) **Legacy Circle Segment Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This is a Legacy item and should not be used.

> From a long dead platform. he who shall not be named on the holy land that is this wiki
>
> — [989onan](https://wiki.resonite.com/User:989onan "User:989onan")

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
| `ExpandLerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to expand the mesh outwards |
| `InnerCircle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this mesh has an inner circle. |
| `RadiusStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the inner side of the segments to the center. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick the segments are from the circle center. |
| `MainSegmentArc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The main segment arc from the dead platform. |
| `SeparationAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far apart the segments should be. |
| `MenuMainSegmentArc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the main segment should be. |
| `CircleItemCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many segments there are. |
| `MenuRadiusStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where the menu starts on a circle in degrees. |
| `MenuThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick the menu items are from circle center. |
| `FillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what color to fill the segments with. |
| `OutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What color the outline of the segments should be. |
| `CircleItemOverrides` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacyCircleSegmentMesh.MenuSegment](https://wiki.resonite.com/Component:LegacyCircleSegmentMesh#MenuSegment)** | Custom list of segments to use. |
| `IndependentSegments` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacyCircleSegmentMesh.MenuSegment](https://wiki.resonite.com/Component:LegacyCircleSegmentMesh#MenuSegment)** | Custom list of independent segments to use. |
| `OutlineWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the item outlines. |

Fields
Collapse

## MenuSegement

| Name | Type | Description |
| --- | --- | --- |
| `RadiusStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the circle center before this segment's inner arc. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick this segment is from the circle center. |
| `AngleStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where this menu item starts in degrees on a circle. |
| `ArcLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of the circle in degrees this menu item takes up. |
| `OverrideColor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to override the root menu color with the one specified in here. |
| `FillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The fill color to use if overriding |
| `OutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The outline color to use if overriding. |

Fields

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Just don't.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyCircleSegmentMesh&oldid=99012](https://wiki.resonite.com/index.php?title=Component:LegacyCircleSegmentMesh&oldid=99012)"

Contents