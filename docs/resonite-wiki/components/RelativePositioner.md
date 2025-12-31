# Component:RelativePositioner

> Source: https://wiki.resonite.com/Component:RelativePositioner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RelativePositioner&diff=95474) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9b/RelativePositionerComponent.png/510px-RelativePositionerComponent.png)](https://wiki.resonite.com/File:RelativePositionerComponent.png) **Relative Positioner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RelativePositioner** component puts the slot its attached to in a position based on the Bounding box and position of `Reference`. Optionally deleting the component on an update when the slot is positioned successfully.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to Relative position to. |
| `ReferenceBoundsSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to calculate the Bounding box of `Reference` in. |
| `ReferenceAnchor` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How far away from the center of the `Reference`'s Bounding box based on size. (1,1,1) puts this slot at the positive corner in global space of `Reference`'s Bounding box and (0,0,0) put it at `Reference`'s center Bounding box point. |
| `ReferenceOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to add to the slot position after Bounding box positioning. |
| `DestroyAfterDone` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to destroy this component after update and positioning was successfully done due to needed fields not being null. |
| `_target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of this slot to drive. |

Fields
Collapse

## Usage

Attach to a slot and provide a `Reference` in order for this component to do a valid position and optionally delete itself within that update.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RelativePositioner&oldid=95474](https://wiki.resonite.com/index.php?title=Component:RelativePositioner&oldid=95474)"

Contents