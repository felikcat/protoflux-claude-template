# Component:TrackerController

> Source: https://wiki.resonite.com/Component:TrackerController

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cb/TrackerControllerComponent.png/510px-TrackerControllerComponent.png)](https://wiki.resonite.com/File:TrackerControllerComponent.png) **Tracker Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TrackerController** component is an internally used component that triggers a pair of sync Delegates when a device is added to the user's list of tracked devices with position and rotation.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PositionStreamConfigurator` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >, [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The Sync delegate to call with the created tracked device's position stream and "2" as a number when a device is added. |
| `RotationStreamConfigurator` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >, [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The Sync delegate to call with the created tracked device's rotation stream and "2" as a number when a device is added. |

Fields
Collapse

## Examples

Automatically attached to the root of a user slot when they spawn.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TrackerController&oldid=95775](https://wiki.resonite.com/index.php?title=Component:TrackerController&oldid=95775)"

Contents