# Component:UserRefToSyncRefAdapter

> Source: https://wiki.resonite.com/Component:UserRefToSyncRefAdapter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7a/UserRefToSyncRefAdapterComponent.png/510px-UserRefToSyncRefAdapterComponent.png)](https://wiki.resonite.com/File:UserRefToSyncRefAdapterComponent.png) **User Ref To Sync Ref Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserRefToSyncRefAdapter** component takes a UserRef type and drives a user ref field with what it has inside of it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The ref to get a user from. |
| `TargetReference` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") < [User](https://wiki.resonite.com/Type:User "Type:User") >** | The field to drive with what user `User` refers to. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to the field `TargetReference` will update the value of `User`. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |

Fields
Collapse

## Usage

Attach to a slot and provide values for all fields in order for this component to work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserRefToSyncRefAdapter&oldid=96505](https://wiki.resonite.com/index.php?title=Component:UserRefToSyncRefAdapter&oldid=96505)"

Contents