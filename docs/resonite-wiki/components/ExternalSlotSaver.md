# Component:ExternalSlotSaver

> Source: https://wiki.resonite.com/Component:ExternalSlotSaver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2b/ExternalSlotSaverComponent.png/510px-ExternalSlotSaverComponent.png)](https://wiki.resonite.com/File:ExternalSlotSaverComponent.png) **External Slot Saver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The ExternalSlotSaver will ensure that the `TargetSlot` is saved as a child of the slot this component is on if the slot isn't already in the hierarchy.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to target when saving. |
| `SaveActiveSelfOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | When not null, save this rather than `TargetSlot`'s current active self value. |
| `SaveLocalPositionOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | When not null, save this rather than `TargetSlot`'s current position value. |
| `SaveLocalRotationOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | When not null, save this rather than `TargetSlot`'s current rotation value. |
| `SaveLocalScaleOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | When not null, save this rather than `TargetSlot`'s current scale value. |
| `IgnoreWhenNonPersistentSelf` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to not save the external slot if we are non persistent ourselves. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ExternalSlotSaver&oldid=93804](https://wiki.resonite.com/index.php?title=Component:ExternalSlotSaver&oldid=93804)"

Contents