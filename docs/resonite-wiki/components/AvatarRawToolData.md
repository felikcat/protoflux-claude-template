# Component:AvatarRawToolData

> Source: https://wiki.resonite.com/Component:AvatarRawToolData

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarRawToolData&diff=93916) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0c/AvatarRawToolDataComponent.png/510px-AvatarRawToolDataComponent.png)](https://wiki.resonite.com/File:AvatarRawToolDataComponent.png) **AvatarRawToolData** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarRawToolData** component is used to read controller data associated with [RawDataTools](https://wiki.resonite.com/Component:RawDataTool "Component:RawDataTool") from.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ControllerSide` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | The side to read data from the user's controller for. |
| `PressingPrimary` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is pressing Primary |
| `PressingSecondary` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is pressing Secondary. |
| `PressingGrab` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is pressing the grab button |
| `PrimaryStrength` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The strength the user is pressing Primary. |
| `SecondaryAxis` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | What direction the user is moving their secondary button joystick |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user this is reading data and getting streams from. |
| `_strengthStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The stream to get `PrimaryStrength`'s value from |
| `_axisStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The stream to get `SecondaryAxis`'s value from. |
| `_primaryStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The stream to get `PressingPrimary`'s value from. |
| `_secondaryStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The stream to get `PressingSecondary`'s value from. |
| `_grabStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The stream to get `PressingGrab`'s value from. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarRawToolData&oldid=93916](https://wiki.resonite.com/index.php?title=Component:AvatarRawToolData&oldid=93916)"

Contents