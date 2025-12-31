# Component:SlotRaycastTransferPortal

> Source: https://wiki.resonite.com/Component:SlotRaycastTransferPortal

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ef/SlotRaycastTransferPortalComponent.png/510px-SlotRaycastTransferPortalComponent.png)](https://wiki.resonite.com/File:SlotRaycastTransferPortalComponent.png) **Slot Raycast Transfer Portal** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SlotRaycastTransferPortal** acts very similarly to the [Component:MeshUVRaycastPortal](https://wiki.resonite.com/Component:MeshUVRaycastPortal "Component:MeshUVRaycastPortal") except that it works on colliders hitting a slot hiearchy to another slot rather than just a mesh and a camera.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Exit` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to send the raycast through if it hits this slot's hierarchy, converting the hit point / direction in this component slot's local space to the space of the slot specified here. |
| `OverrideHitTriggers` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether to override if a laser coming through will hit triggers and what to override it with. |
| `Filter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The filter we should apply if a raycast comes through this portal? |
| `FilterMode` | **[FilterCombineMode](https://wiki.resonite.com/Type:FilterCombineMode "Type:FilterCombineMode")** | If a raycast being transfered has its own filter, how should we combine it with `Filter` if it exists?. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:MeshUVRaycastPortal](https://wiki.resonite.com/Component:MeshUVRaycastPortal "Component:MeshUVRaycastPortal")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SlotRaycastTransferPortal&oldid=95669](https://wiki.resonite.com/index.php?title=Component:SlotRaycastTransferPortal&oldid=95669)"

Contents