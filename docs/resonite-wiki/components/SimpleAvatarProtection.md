# Component:SimpleAvatarProtection

> Source: https://wiki.resonite.com/Component:SimpleAvatarProtection

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SimpleAvatarProtection&diff=99191) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/be/SimpleAvatarProtectionComponent.png/510px-SimpleAvatarProtectionComponent.png)](https://wiki.resonite.com/File:SimpleAvatarProtectionComponent.png) **SimpleAvatarProtection** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

SimpleAvatarProtection prevents other users from wearing an avatar or saving it.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | _direct_ **[CloudUserRef](https://wiki.resonite.com/index.php?title=Type:CloudUserRef&action=edit&redlink=1 "Type:CloudUserRef (page does not exist)")** | The user who is permitted to use the avatar. |
| `ReassignUserOnPackageImport` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | See [ResonitePackage#Simple\_Avatar\_Protection\_handling](https://wiki.resonite.com/ResonitePackage#Simple_Avatar_Protection_handling "ResonitePackage"). |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnRemoveSingleInstance:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Removes this component as long as the activating user is allowed to do so. |
| `OnRemoveAllInstances:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Removes components in the hiearchy as long as the activating user is allowed to do so. |

Triggers
Collapse

## Behavior

When attached anywhere on an avatar, the SimpleAvatarProtection component prevents all users, other than the single user listed on the component, from saving the avatar, grabbing materials off of it, or equipping it.

The component is automatically attached to an avatar if "Protect Avatar" is checked in the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator") when creating it.

All instances of SimpleAvatarProtection on an avatar can be removed _by its owner_ by clicking the "Remove All Instances" button. No other user can remove the component. This is useful if you are trying to clear protection from an avatar, but cannot remember where the component was; you can simply add another instance and remove them all at once.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SimpleAvatarProtection&oldid=99191](https://wiki.resonite.com/index.php?title=Component:SimpleAvatarProtection&oldid=99191)"

Contents