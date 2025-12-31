# Component:AvatarUserReferenceAssigner

> Source: https://wiki.resonite.com/Component:AvatarUserReferenceAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarUserReferenceAssigner&diff=97401) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2f/AvatarUserReferenceAssignerComponent.png/510px-AvatarUserReferenceAssignerComponent.png)](https://wiki.resonite.com/File:AvatarUserReferenceAssignerComponent.png) **Avatar User Reference Assigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarUserReferenceAssigner** component is used to assign the [user](https://wiki.resonite.com/User "User") reference to a list of targets (depending on the `AssignMode`). This component activates only when in the [slot](https://wiki.resonite.com/Slot "Slot") hierarchy of an [Avatar](https://wiki.resonite.com/Avatar "Avatar") and when a user equips it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AssignMode` | **[AvatarUserReferenceAssigner.Mode](https://wiki.resonite.com/Component:AvatarUserReferenceAssigner#Mode)** | How to use the list when assigning users to User storage fields. |
| `References` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [User](https://wiki.resonite.com/Type:User "Type:User") >** | The references to scan through when assigning. |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `WhiteList` | 0 | Assign and unassign the values of only the User storage fields specified in `References` |
| `AutoscanWithBlacklist` | 1 | Assign and Unassign the values of every User storage field in the avatar hierarchy except for the ones specified in `References` |

Values

## Usage

This is often used with assigning the [user](https://wiki.resonite.com/User "User") reference to [nameplates](https://wiki.resonite.com/Nameplate#User_Referencing "Nameplate"), and the components within.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarUserReferenceAssigner&oldid=97401](https://wiki.resonite.com/index.php?title=Component:AvatarUserReferenceAssigner&oldid=97401)"

Contents