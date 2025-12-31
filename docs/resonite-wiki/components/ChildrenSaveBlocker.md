# Component:ChildrenSaveBlocker

> Source: https://wiki.resonite.com/Component:ChildrenSaveBlocker

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2b/ChildrenSaveBlockerComponent.png/510px-ChildrenSaveBlockerComponent.png)](https://wiki.resonite.com/File:ChildrenSaveBlockerComponent.png) **ChildrenSaveBlocker** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ChildrenSaveBlocker** component prevents the slot's children from being saved with the slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

When attached to a slot, the children of the slot will not be saved when the slot is part of an item being saved. The slot itself will still be saved.

## Examples

There are a few cases where this component can be useful:

- A room or workspace for user holding where items that are not persistent may find themselves in. This component can be used to save the workspace (and thus retain functionality) but not the items in it.
- Placed on a slot with a [SnapTarget](https://wiki.resonite.com/Component:SnapTarget "Component:SnapTarget") to save snapping behavior while not saving any items placed in the snap target.
- Placed on a slot with a [GrabbableReceiverSurface](https://wiki.resonite.com/Component:GrabbableReceiverSurface "Component:GrabbableReceiverSurface") or its `OverrideParent` to save receiver behavior while not saving any items on the surface.

## See also

- [GrabbableSaveBlock](https://wiki.resonite.com/index.php?title=Component:GrabbableSaveBlock&action=edit&redlink=1 "Component:GrabbableSaveBlock (page does not exist)") for blocking saves of grabbable items.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ChildrenSaveBlocker&oldid=104578](https://wiki.resonite.com/index.php?title=Component:ChildrenSaveBlocker&oldid=104578)"

Contents