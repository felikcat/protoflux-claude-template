# Component:SettingActionProxy

> Source: https://wiki.resonite.com/Component:SettingActionProxy

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:SettingActionProxy\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SettingActionProxy%601Component.png "File:SettingActionProxy`1Component.png") **Setting Action Proxy\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SettingActionProxy** component is used to trigger an action on a subsetting under the component of type **S** which would be globally registered in the world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ActionName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the action being triggered. |
| `SubsettingGetter` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the sync delegate method being triggered. |
| `SubsettingKey` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The key being used to find the sub setting being triggered. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Trigger:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | triggers the target specified by this component's values and generic typing. |

Triggers
Collapse

## Usage

Used in the settings menu and only works in user space.

## Examples

Settings menu UI.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingActionProxy&oldid=99188](https://wiki.resonite.com/index.php?title=Component:SettingActionProxy&oldid=99188)"

Contents