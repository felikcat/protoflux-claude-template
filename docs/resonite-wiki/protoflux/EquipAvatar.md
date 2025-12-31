# ProtoFlux:EquipAvatar

> Source: https://wiki.resonite.com/ProtoFlux:EquipAvatar

Equip Avatar

\*

Next

User

AvatarRoot

DestroyOld

Avatars

Equip Avatar is a ProtoFlux node that allows for making a [User](https://wiki.resonite.com/Type:User "Type:User") Equip an [Avatar](https://wiki.resonite.com/Avatar "Avatar"). A bit of caution should be used when using this node, since making people equip an avatar against their will without proper forewarning can be considered distasteful at best.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to make the provided User ( [User](https://wiki.resonite.com/Type:User "Type:User")) equip the provided AvatarRoot ( [Slot](https://wiki.resonite.com/Slot "Slot")).

### User ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user that should equip the provided AvatarRoot ( [Slot](https://wiki.resonite.com/Slot "Slot")).

### AvatarRoot ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The [Avatar](https://wiki.resonite.com/Avatar "Avatar") the provided User ( [User](https://wiki.resonite.com/Type:User "Type:User")) should equip. This slot is usually where the [AvatarRoot](https://wiki.resonite.com/Component:AvatarRoot "Component:AvatarRoot") component would be on an avatar which usually resides with the [VRIK](https://wiki.resonite.com/Component:VRIK "Component:VRIK").

### DestroyOld ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the avatar the user was previously wearing should be destroyed. Only use this when nessary, because the avatar will be gone _forever_ from the world when deleted.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) was called and the provided User ( [User](https://wiki.resonite.com/Type:User "Type:User")) has equipped the provided AvatarRoot ( [Slot](https://wiki.resonite.com/Slot "Slot")).

## Examples

- [How to use an Equip Avatar node.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Equip_Avatar.webp "File:Protoflux example Equip Avatar.webp")

How to use an Equip Avatar node.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EquipAvatar&oldid=109727](https://wiki.resonite.com/index.php?title=ProtoFlux:EquipAvatar&oldid=109727)"

Contents