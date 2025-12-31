# Component:AvatarSlotEquippedToggle

> Source: https://wiki.resonite.com/Component:AvatarSlotEquippedToggle

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarSlotEquippedToggle&diff=92255) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0d/AvatarSlotEquippedToggleComponent.png/510px-AvatarSlotEquippedToggleComponent.png)](https://wiki.resonite.com/File:AvatarSlotEquippedToggleComponent.png) **AvatarSlotEquippedToggle** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarSlotEquippedToggle** component drives one or two booleans to a state depending on if an [Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") is equipped or not.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ObjectSlot` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") >** | The Avatar Object Slot to monitor for equipping status. |
| `EquippedDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Drives the target bool to true when `ObjectSlot` is equipped. Otherwise false. |
| `DequippedDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Drives the target bool to false when `ObjectSlot` is equipped. Otherwise true. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarSlotEquippedToggle&oldid=92255](https://wiki.resonite.com/index.php?title=Component:AvatarSlotEquippedToggle&oldid=92255)"

Contents