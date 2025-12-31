# Component:ExternalSlotDuplicator

> Source: https://wiki.resonite.com/Component:ExternalSlotDuplicator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/17/ExternalSlotDuplicatorComponent.png/510px-ExternalSlotDuplicatorComponent.png)](https://wiki.resonite.com/File:ExternalSlotDuplicatorComponent.png) **External Slot Duplicator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ExternalSlotDuplicator** component parents `TargetSlot` under itself when this component is duplicated. If this component is parented under a larger hiearchy, the slot will only be parented if it's not anywhere under this larger hiearchy or this component's hiearchy. When the slot is parented back under this component, any non null specified transform values for this component are applied to the slot.

If `DoNotRestoreOriginalTransform` is enabled, it will parent the slot back where it came from and restore the original local transform values after duplication.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to parent and write values for during duplication. |
| `LocalPositionOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The local position to apply to `TargetSlot` when parenting under this slot during duplication if this is not null. |
| `LocalRotationOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The local rotation to apply to `TargetSlot` when parenting under this component's slot during duplication if this is not null. |
| `LocalScaleOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The local scale to apply to `TargetSlot` when parenting under this component's slot during duplication if this is not null. |
| `ActiveSelfOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The active state to apply to `TargetSlot`'s active field when parenting under this component's slot during duplication if this is not null. |
| `DoNotRestoreOriginalTransform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to parent the slot back where it came from after duplication, Undoing all overrides and setting all values back to their originals. |

Fields
Collapse

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ExternalSlotDuplicator&oldid=94523](https://wiki.resonite.com/index.php?title=Component:ExternalSlotDuplicator&oldid=94523)"

Contents