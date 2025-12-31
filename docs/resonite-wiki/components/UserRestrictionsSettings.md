# Component:UserRestrictionsSettings

> Source: https://wiki.resonite.com/Component:UserRestrictionsSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0b/UserRestrictionsSettingsComponent.png/510px-UserRestrictionsSettingsComponent.png)](https://wiki.resonite.com/File:UserRestrictionsSettingsComponent.png) **User Restrictions Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserRestrictionsSettings** component is found in the user space and contains all blocked user entries. this is a good way to handle blocked users until they fix the regression of no longer having a blocked users list introduced in the settings update.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Entries` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRestrictionsSettings.Entry](https://wiki.resonite.com/Component:UserRestrictionsSettings#Entry)** | A list of blocked users. |

Fields
Collapse

## Entry

| Name | Type | Description |
| --- | --- | --- |
| `BlockType` | **[BlockType](https://wiki.resonite.com/Type:BlockType "Type:BlockType")** | The kind of block type you did against this user. |
| `IsFullyBanned` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is fully banned by you or not from your sessions and worlds. |
| `Username` | **[string](https://wiki.resonite.com/Type:String "Type:String")** | The username of the user. |
| `UserId` | **[string](https://wiki.resonite.com/Type:String "Type:String")** | The user ID of the user. |
| `MachineIDs` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of machine ids this user may have. |
| `ExtraIds` | _direct_ **[SyncFieldDictionary\`2](https://wiki.resonite.com/index.php?title=Type:SyncFieldDictionary%602&action=edit&redlink=1 "Type:SyncFieldDictionary`2 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String"), [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of extra machine ids for this user. |
| `BannedWorldList` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of worlds of yours the user is banned from. |

Fields

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserRestrictionsSettings&oldid=106608](https://wiki.resonite.com/index.php?title=Component:UserRestrictionsSettings&oldid=106608)"

Contents