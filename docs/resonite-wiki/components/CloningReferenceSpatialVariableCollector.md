# Component:CloningReferenceSpatialVariableCollector

> Source: https://wiki.resonite.com/Component:CloningReferenceSpatialVariableCollector

Collapse **Component image**

[File:CloningReferenceSpatialVariableCollector\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=CloningReferenceSpatialVariableCollector%601Component.png "File:CloningReferenceSpatialVariableCollector`1Component.png") **Cloning Reference Spatial Variable Collector\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Cloning Reference Spatial Variable Collector\`1** component is part of the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. It works similarly to [ReferenceSpatialVariableCollector](https://wiki.resonite.com/Component:ReferenceSpatialVariableCollector "Component:ReferenceSpatialVariableCollector"), but specifically for components. For each component it finds at the point, it will create & maintain a duplicate. It can duplicate either just the component itself or the whole Slot it's on. The duplicates can be made Local only (it's your responsibility to make sure that the target list can reference local elements). It will never clone spatial variables present on the slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CloneParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to parent cloned elements to. |
| `MakeClonesLocal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether cloned items should be on the local machine rather than networked. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable being sampled. |
| `Mode` | **[CloneMode](https://wiki.resonite.com/index.php?title=Type:CloneMode&action=edit&redlink=1 "Type:CloneMode (page does not exist)")** | How to clone elements this samples. |
| `ReferenceList` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[ISyncRefList\`1](https://wiki.resonite.com/index.php?title=Type:ISyncRefList%601&action=edit&redlink=1 "Type:ISyncRefList`1 (page does not exist)") <T>** | The list of references this component has sampled at the point of the slot it is on. |

Fields
Collapse

## Usage

Attach to a slot and bring near a set of [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") to get a list of references. don't forget to add a variable name and reference list.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CloningReferenceSpatialVariableCollector&oldid=101126](https://wiki.resonite.com/index.php?title=Component:CloningReferenceSpatialVariableCollector&oldid=101126)"

Contents