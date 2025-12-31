# Component:DebugSettingListener

> Source: https://wiki.resonite.com/Component:DebugSettingListener

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/DebugSettingListenerComponent.png/510px-DebugSettingListenerComponent.png)](https://wiki.resonite.com/File:DebugSettingListenerComponent.png) **Debug Setting Listener** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugSettingListener** component is used for debugging settings changes as part of the settings system.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CurrentValue` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Setting path to check. |
| `SettingChangeCounter` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many times the Setting has been changed. |

Fields
Collapse

## Usage

Debug.

## Examples

Debug.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugSettingListener&oldid=96425](https://wiki.resonite.com/index.php?title=Component:DebugSettingListener&oldid=96425)"

Contents