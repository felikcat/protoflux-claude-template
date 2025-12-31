# Component:SettingSync

> Source: https://wiki.resonite.com/Component:SettingSync

Collapse **Component image**

[File:SettingSync\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SettingSync%601Component.png "File:SettingSync`1Component.png") **Setting Sync\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Is an alternative version of [SettingValueSync\`2](https://wiki.resonite.com/Component:SettingValueSync%602 "Component:SettingValueSync`2").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SyncingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user to get the setting from. |
| `SettingPath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The setting or setting group to get a value for. This is a path separated by ".". |
| `LocalChangeAction` | **[LocalChange](https://wiki.resonite.com/index.php?title=Type:LocalChange&action=edit&redlink=1 "Type:LocalChange (page does not exist)")** | How to handle changes to the value of `TargetField` and whether to update the setting value for the local value or not if they trigger it to change in the world. |
| `TargetField` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The field to put the setting value into, can also write back to the setting if the world is unsafe or the setting allows for the world to write it and `LocalChangeAction` is set for it. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingSync&oldid=106557](https://wiki.resonite.com/index.php?title=Component:SettingSync&oldid=106557)"

Contents