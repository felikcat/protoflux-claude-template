# Component:ReferenceSpatialVariableCollector

> Source: https://wiki.resonite.com/Component:ReferenceSpatialVariableCollector

Collapse **Component image**

[File:ReferenceSpatialVariableCollector\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ReferenceSpatialVariableCollector%601Component.png "File:ReferenceSpatialVariableCollector`1Component.png") **Reference Spatial Variable Collector\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Reference Spatial Variable Collector\`1** component is specifically for reference types This drives a list of references, filling it with all the found spatial variables. It does this by reading all spatial variables of the reference type matching this one, and in range, and puts them into the referenced list.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ReferenceList` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncRefList\`1](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1") <T>** | The list to populate with the spatial variables of all spatial fields intersecting the point that is the slot this component is on. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variable to sample for. |
| `DefaultTarget` | **T** | The value to default to when no references can be sampled at all. |

Fields
Collapse

## Usage

Attach to a slot which will be used as the point to sample from. give a target list to drive, and the list will populate with found values

## Examples

This can be used to collect slots and put them into a list of bones on a mesh, or to apply audio effects to [Component:AudioListeners](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener").

## See Also

- [Component:AudioListener](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceSpatialVariableCollector&oldid=101129](https://wiki.resonite.com/index.php?title=Component:ReferenceSpatialVariableCollector&oldid=101129)"

Contents