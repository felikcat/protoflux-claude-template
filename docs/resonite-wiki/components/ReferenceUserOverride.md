# Component:ReferenceUserOverride

> Source: https://wiki.resonite.com/Component:ReferenceUserOverride

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceUserOverride&diff=97703) which are not marked for translation.

This is a component that allows you to locally change a reference on a value. Changing the value locally for yourself or others so that an item or world element is different depending on who's viewing it.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/39/ReferenceUserOverride%601Component.png/510px-ReferenceUserOverride%601Component.png)](https://wiki.resonite.com/File:ReferenceUserOverride%601Component.png) **Reference User Override\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | The value to drive locally for every user |
| `Default` | **T** | The content of this value will be inside of `Target` for every user locally unless otherwise specified by an [Override](https://wiki.resonite.com/Component:ReferenceUserOverride#Override) inside of the `_overrides` bag. |
| `CreateOverrideOnWrite` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When flux or any other means tries to set the value of target from someone's machine, create an [Override](https://wiki.resonite.com/Component:ReferenceUserOverride#Override) for them in `_overrides` bag. |
| `PersistentOverrides` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to save the overrides or not when the component is part of a hierarchy being saved. This is useful to turn on when an item should have overrides |
| `_overrides` | _[unordered list](https://wiki.resonite.com/Type:SyncBag%601 "Type:SyncBag`1")_ of **[ReferenceUserOverride\`1.Override](https://wiki.resonite.com/Component:ReferenceUserOverride#Override) <T>** | A bag of [Overrides](https://wiki.resonite.com/Component:ReferenceUserOverride#Override) that are read to make local changes to the value referenced by `Target` |

Fields
Collapse

## Override

| Name | Type | Description |
| --- | --- | --- |
| `User` | [UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef") | The [User](https://wiki.resonite.com/Type:User "Type:User") that should see `Value`'s content inside of `Target` locally instead of `Default`'s content |
| `Value` | **T** | The value that `User` should see target driven to locally. |

Fields

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceUserOverride&oldid=97703](https://wiki.resonite.com/index.php?title=Component:ReferenceUserOverride&oldid=97703)"

Contents