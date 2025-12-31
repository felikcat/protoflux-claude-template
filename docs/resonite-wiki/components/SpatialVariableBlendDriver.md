# Component:SpatialVariableBlendDriver

> Source: https://wiki.resonite.com/Component:SpatialVariableBlendDriver

Collapse **Component image**

[File:SpatialVariableBlendDriverComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SpatialVariableBlendDriverComponent.png "File:SpatialVariableBlendDriverComponent.png") **Spatial Variable Blend Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Spatial Variable Blend Driver** component combines with the [CloningReferenceSpatialVariableCollector](https://wiki.resonite.com/Component:CloningReferenceSpatialVariableCollector "Component:CloningReferenceSpatialVariableCollector") component. If this is on a field on a spatial variable component which is driven by this component, the cloned version will be driven with the current blend weight for that clone. This is used for the BlendWeight for the new reverb zones. For more info on making reverb zones, see [Component:AudioListener](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BlendWeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | used for proportional blending and priority computation |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SpatialVariableBlendDriver&oldid=101128](https://wiki.resonite.com/index.php?title=Component:SpatialVariableBlendDriver&oldid=101128)"

Contents