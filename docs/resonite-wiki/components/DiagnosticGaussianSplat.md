# Component:DiagnosticGaussianSplat

> Source: https://wiki.resonite.com/Component:DiagnosticGaussianSplat

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/DiagnosticGaussianSplatComponent.png/510px-DiagnosticGaussianSplatComponent.png)](https://wiki.resonite.com/File:DiagnosticGaussianSplatComponent.png) **Diagnostic Gaussian Splat** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Diagnostic Gaussian Splat** component is used to render diagnostic info on [Gaussian Splats](https://wiki.resonite.com/Gaussian_Splat "Gaussian Splat").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `SplatColorProfile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `Splats` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DiagnosticGaussianSplat.SplatData](https://wiki.resonite.com/Component:DiagnosticGaussianSplat#SplatData)** | A list of splats to render diagnostics for. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeGaussianSplat:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DiagnosticGaussianSplat&oldid=113571](https://wiki.resonite.com/index.php?title=Component:DiagnosticGaussianSplat&oldid=113571)"

Contents