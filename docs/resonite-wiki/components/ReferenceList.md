# Component:ReferenceList

> Source: https://wiki.resonite.com/Component:ReferenceList

Collapse **Component image**

[File:ReferenceList\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ReferenceList%601Component.png "File:ReferenceList`1Component.png") **Reference List\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Reference List\`1** component acts as a way to store a list of references as a stand alone component. like a [ReferenceField](https://wiki.resonite.com/Component:ReferenceField "Component:ReferenceField"), but for a list of items of the same type.

This component does not provide a way to index through its items. If you need this functionality, consider using a [ReferenceMultiplexer](https://wiki.resonite.com/Component:ReferenceMultiplexer "Component:ReferenceMultiplexer") Instead.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `References` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **T** | The stored reference list. |

Fields
Collapse

## Usage

Can be used with [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables").

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceList&oldid=112793](https://wiki.resonite.com/index.php?title=Component:ReferenceList&oldid=112793)"

Contents