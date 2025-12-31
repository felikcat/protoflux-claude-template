# Component:SettingValueSync

> Source: https://wiki.resonite.com/Component:SettingValueSync

Collapse **Component image**

[File:SettingValueSync\`2Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SettingValueSync%602Component.png "File:SettingValueSync`2Component.png") **Setting Value Sync\`2** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SettingValueSync** component allows for reading (And sometimes writing) a setting from a particular `SyncingUser` for the purpose of changing an item/world's appearance or behavior depending on that settings value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SyncingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to get the setting from. |
| `SettingName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The setting or setting group to get a value for. This is a path separated by ".". |
| `TargetField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to put the setting value into, can also write back to the setting if the world is unsafe or the setting allows for the world to write it. |
| `SubsettingGetter` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The subsetting method name to use to get a subsetting. |
| `SubsettingKey` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The key to pass to the subsetting getter method found under the name specified by `SubsettingGetter` in order to get a subsetting. |

Fields
Collapse

## Usage

Attach to a slot and provide a setting path (`SettingName`) and a `SyncingUser` to read from in order to read values. For subsettings like audio devices or trackers a name provided to `SubsettingGetter` of a [SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter") and a key to use in `SubsettingKey` is needed.

## Examples

Can be used to make an item/avatar/world inform the user that an item won't look correct, or will behave differently depending on that user's settings.

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingValueSync&oldid=99149](https://wiki.resonite.com/index.php?title=Component:SettingValueSync&oldid=99149)"

Contents