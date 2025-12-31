# Component:SettingValueActionProxy

> Source: https://wiki.resonite.com/Component:SettingValueActionProxy

Collapse **Component image**

[File:SettingValueActionProxy\`2Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SettingValueActionProxy%602Component.png "File:SettingValueActionProxy`2Component.png") **Setting Value Action Proxy\`2** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SettingValueActionProxy** component is used to trigger an action while passing a value to it on a subsetting under the component of type **S** which would be globally registered in the world.

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
| ``Trigger:Action`1<T>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | X | triggers the target, while passing a value of type **T**, which the target specified by this component's values and generic typing. |

Triggers
Collapse

## Usage

Not to be used directly by the user.

## Examples

Is used in the session tab in the dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SettingValueActionProxy&oldid=99197](https://wiki.resonite.com/index.php?title=Component:SettingValueActionProxy&oldid=99197)"

Contents