# Component:TransferGrabbable

> Source: https://wiki.resonite.com/Component:TransferGrabbable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/da/TransferGrabbableComponent.png/510px-TransferGrabbableComponent.png)](https://wiki.resonite.com/File:TransferGrabbableComponent.png) **Transfer Grabbable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Transfer Grabbable is a component that is used to mark objects that undergo [Transfer grabbing](https://wiki.resonite.com/Transfer_grabbing "Transfer grabbing"), but only while in [Userspace](https://wiki.resonite.com/Userspace "Userspace"). The grabber during this process saves the object into memory including materials, then simulates a paste as it puts the object into the target world.

If the world does not allow transferring to it, the `_indicatorMaterial` material will replace materials on the object and light up red. Will restore the materials back if transferring is allowed to the target world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PasteOnGrab` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to trigger a paste event in userspace when transfering the object to user space. does not affect when releasing. |
| `_indicatorMaterial` | **[FresnelMaterial](https://wiki.resonite.com/Component:FresnelMaterial "Component:FresnelMaterial")** | The indicator material to use when transfering to worlds. |

Fields
Collapse

## Usage

Not intended to be used directly

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TransferGrabbable&oldid=104631](https://wiki.resonite.com/index.php?title=Component:TransferGrabbable&oldid=104631)"

Contents