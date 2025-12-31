# Component:QuadArrayMesh

> Source: https://wiki.resonite.com/Component:QuadArrayMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:QuadArrayMesh&diff=98026) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f9/QuadArrayMeshComponent.png/510px-QuadArrayMeshComponent.png)](https://wiki.resonite.com/File:QuadArrayMeshComponent.png) **Quad Array Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Quad array mesh makes a bunch of quads with defined positions, rotations, vertex colors, and UV coordinates which are rendered as one mesh. This is made from Quad brushes which can be found in the resonite essentials folder.

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
| `Points` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | An array inaccessible without [Mods](https://wiki.resonite.com/Mods "Mods") that defines where each quad for this mesh should be in local space. |
| `Sizes` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | An array inaccessible without [Mods](https://wiki.resonite.com/Mods "Mods") that defines the scale for each quad for this mesh in local space. |
| `Rotations` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | An array inaccessible without [Mods](https://wiki.resonite.com/Mods "Mods") that defines the rotation for each quad for this mesh in local space. |
| `Colors` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Color](https://wiki.resonite.com/Type:Color "Type:Color")** | An array inaccessible without [Mods](https://wiki.resonite.com/Mods "Mods") that defines the vertex colors for each quad for this mesh. |
| `ColorsProfile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile of each quad. |
| `UVs` | _[array](https://wiki.resonite.com/Type:SyncArray%601 "Type:SyncArray`1")_ of **[Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4")** | An array inaccessible without [Mods](https://wiki.resonite.com/Mods "Mods") xy of each element defines the center of each quad and zw defines the uv scales of each quad on a texture/material. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

This component is not usually used directly

## Examples

Made by Quad brushes in the resonite essentials folder.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:QuadArrayMesh&oldid=98026](https://wiki.resonite.com/index.php?title=Component:QuadArrayMesh&oldid=98026)"

Contents