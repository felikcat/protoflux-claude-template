# Component:InteractionHandlerStreamDriver

> Source: https://wiki.resonite.com/Component:InteractionHandlerStreamDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:InteractionHandlerStreamDriver&diff=90862) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9a/InteractionHandlerStreamDriverComponent.png/510px-InteractionHandlerStreamDriverComponent.png)](https://wiki.resonite.com/File:InteractionHandlerStreamDriverComponent.png) **InteractionHandlerStreamDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InteractionHandlerStreamDriver** component uses streaming data from the [ValueStream](https://wiki.resonite.com/index.php?title=Component:ValueStream&action=edit&redlink=1 "Component:ValueStream (page does not exist)") component (seen in the [user Inspector](https://wiki.resonite.com/User_Inspector "User Inspector")) to control the interaction (such as [lasers](https://wiki.resonite.com/Component:Laser "Component:Laser")) on a [user's](https://wiki.resonite.com/User "User") [avatar](https://wiki.resonite.com/Avatar "Avatar") or [Userspace](https://wiki.resonite.com/Userspace "Userspace").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Side` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | The side to get the data. |
| `PrimaryBlockedStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The value interaction data currently being blocked. (Primary) |
| `SecondaryBlockedStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The value interaction data currently being blocked. (Secondary) |
| `LaserActiveStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The streamed data for this interaction. |
| `ShowLaserToOthersStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Shows the laser data for the other stream. |
| `LaserTargetStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Shows the value for the target of this interaction. |
| `GrabDistanceStream` | **[ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Shows the data of the distance of this interaction. |

Fields
Collapse

## Usage

Used for [lasers](https://wiki.resonite.com/Component:Laser "Component:Laser") and interactions.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractionHandlerStreamDriver&oldid=90862](https://wiki.resonite.com/index.php?title=Component:InteractionHandlerStreamDriver&oldid=90862)"

Contents