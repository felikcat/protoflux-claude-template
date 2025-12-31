# Component:SlicingVolumeVisualizer

> Source: https://wiki.resonite.com/Component:SlicingVolumeVisualizer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/SlicingVolumeVisualizerComponent.png/510px-SlicingVolumeVisualizerComponent.png)](https://wiki.resonite.com/File:SlicingVolumeVisualizerComponent.png) **Slicing Volume Visualizer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SlicingVolumeVisualizer** component is used to visualize the slicer imported with new volumes imported into the game.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VolumeUnlitMaterial](https://wiki.resonite.com/index.php?title=VolumeUnlitMaterial&action=edit&redlink=1 "VolumeUnlitMaterial (page does not exist)") >** | The material to be slicing. |
| `AutoScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to auto scale the visual to fit the object it is slicing. |
| `_renderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The renderer component which this is slicing a mesh for. |
| `_mesh` | **[BoxMesh](https://wiki.resonite.com/Component:BoxMesh "Component:BoxMesh")** | The mesh this visual is slicing. |
| `_collider` | **[BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider")** | The box collider that is used to interact with the slicer this is attached to. |
| `_scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the slicer visual element. |
| `Slicers` | _direct_ **[SyncRelayList\`1](https://wiki.resonite.com/index.php?title=Type:SyncRelayList%601&action=edit&redlink=1 "Type:SyncRelayList`1 (page does not exist)") < [VolumePlaneSlicer](https://wiki.resonite.com/Component:VolumePlaneSlicer "Component:VolumePlaneSlicer") >** | A list of slicers that are slicing the object. |
| `_slicePlanes` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncList\`1](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1") < [SlicePlane](https://wiki.resonite.com/index.php?title=Type:SlicePlane&action=edit&redlink=1 "Type:SlicePlane (page does not exist)") >** | A list of slice planes that are slicing the object. |
| `_highlights` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncList\`1](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1") < [Highlight](https://wiki.resonite.com/index.php?title=Type:Highlight&action=edit&redlink=1 "Type:Highlight (page does not exist)") >** | a list of highlight components for slicing the object. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SlicingVolumeVisualizer&oldid=106558](https://wiki.resonite.com/index.php?title=Component:SlicingVolumeVisualizer&oldid=106558)"

Contents