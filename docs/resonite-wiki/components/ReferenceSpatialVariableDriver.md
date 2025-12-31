# Component:ReferenceSpatialVariableDriver

> Source: https://wiki.resonite.com/Component:ReferenceSpatialVariableDriver

Collapse **Component image**

[File:ReferenceSpatialVariableDriver\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ReferenceSpatialVariableDriver%601Component.png "File:ReferenceSpatialVariableDriver`1Component.png") **Reference Spatial Variable Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Reference Spatial Variable Driver\`1** component gets the closest reference value in the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system and drives a field with it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Drive` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | The field to drive. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variable name to sample for. |
| `DefaultTarget` | **T** | The value to default to when no reference can be sampled. |

Fields
Collapse

## Usage

Attach to a slot and provide a field to drive and a variable name. the slot this component is on acts as the position for sampling variable values.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceSpatialVariableDriver&oldid=101123](https://wiki.resonite.com/index.php?title=Component:ReferenceSpatialVariableDriver&oldid=101123)"

Contents