# Component:VHACD Dialog

> Source: https://wiki.resonite.com/Component:VHACD_Dialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4a/VHACD_DialogComponent.png/510px-VHACD_DialogComponent.png)](https://wiki.resonite.com/File:VHACD_DialogComponent.png) **VHACD Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VHACD\_Dialog** component or V-HACD 2.0 dialog, is used to do a convex hull decomposition on a mesh to make the collision simpler and more performant.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetCollider` | **[MeshCollider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider")** | The collider to simplify. |
| `MergeDoubles` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether to merge double vertices. |
| `Resolution` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | maximum number of voxels generated during the voxelization stage |
| `Depth` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | maximum number of clipping stages. During each split stage, all the model parts (with a concavity higher than the user defined threshold) are clipped according the "best" clipping plane |
| `Concavity` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | maximum concavity |
| `PlaneDownsampling` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | controls the granularity of the search for the "best" clipping plane |
| `ConvexHullDownsampling` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | controls the precision of the convex-hull generation process during the clipping plane selection stage |
| `Alpha` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | controls the bias toward clipping along symmetry planes |
| `Beta` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | controls the bias toward clipping along revolution axes |
| `Gamma` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | maximum allowed concavity during the merge stage |
| `Delta` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | Controls the bias toward maximizing local concavity |
| `PCA` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | enable/disable normalizing the mesh before applying the convex decomposition |
| `Mode` | **[DecompositionMode](https://wiki.resonite.com/Type:DecompositionMode "Type:DecompositionMode")** | how to base the approximate convex decomposition |
| `MaxVerticesPerHull` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | controls the maximum number of vertices per convex-hull |
| `MinVolumePerHull` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | controls the adaptive sampling of the generated convex-hulls |
| `ConvexHullApproximation` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Approximate the convex hulls. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `RunDecomposition:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Activates and starts running the decomposition. |
| `RemoveVisuals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Removes the generated visuals after making a convex hull decomposition. |
| `RemoveHulls:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Delete any generated hulls. |

Triggers
Collapse

## Usage

- [V-HACD 2.0 Github](https://github.com/Unity-Technologies/VHACD)

## Examples

- [V-HACD 2.0 Github](https://github.com/Unity-Technologies/VHACD)

## See Also

- [V-HACD 2.0 Github](https://github.com/Unity-Technologies/VHACD)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VHACD\_Dialog&oldid=100813](https://wiki.resonite.com/index.php?title=Component:VHACD_Dialog&oldid=100813)"

Contents