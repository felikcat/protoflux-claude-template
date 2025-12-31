# Component:GenericSlicer

> Source: https://wiki.resonite.com/Component:GenericSlicer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/40/GenericSlicerComponent.png/510px-GenericSlicerComponent.png)](https://wiki.resonite.com/File:GenericSlicerComponent.png) **Generic Slicer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GenericSlicer** component is used to drive and handle the slicing of materials like volumes and PBS Slice.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Targets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[GenericSlicer.SliceDrive](https://wiki.resonite.com/Component:GenericSlicer#SliceDrive)** | The Slicer Fields on materials to drive. |
| `Space` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The transform space to do slicing in. |
| `_grabbedVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The visual to show and hide when this Slicer is grabbed. |

Fields
Collapse

## SliceDrive

| Name | Type | Description |
| --- | --- | --- |
| `Position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of a material slice entry to drive |
| `Normal` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Normal of a material slice entry to drive |
| `Destroyed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [SliceDrive](https://wiki.resonite.com/Component:GenericSlicer#SliceDrive) >** | The Sync delegate to call when this is destroyed, passing this entry as an argument. |

Fields

## Usage

See [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool").

## Examples

See [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool").

## See Also

- [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GenericSlicer&oldid=97516](https://wiki.resonite.com/index.php?title=Component:GenericSlicer&oldid=97516)"

Contents