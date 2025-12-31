# Component:ColliderEventRelay

> Source: https://wiki.resonite.com/Component:ColliderEventRelay

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7f/ColliderEventRelayComponent.png/510px-ColliderEventRelayComponent.png)](https://wiki.resonite.com/File:ColliderEventRelayComponent.png) **Collider Event Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColliderEventRelay** takes a collider to monitor and sends [ContactEvent](https://wiki.resonite.com/Type:ContactEvent "Type:ContactEvent") messages when certain collisions happen.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Collider` | **[ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider")** | The collider to monitor events for. |
| `ContactStart` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ContactEvent](https://wiki.resonite.com/Type:ContactEvent "Type:ContactEvent")** | The Sync delegate of a certain definition to call when `Collider` starts contact with another collider. |
| `ContactStay` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ContactEvent](https://wiki.resonite.com/Type:ContactEvent "Type:ContactEvent")** | The Sync delegate of a certain definition to call when `Collider` stays in contact with another collider. Is called every frame. |
| `ContactEnd` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ContactEvent](https://wiki.resonite.com/Type:ContactEvent "Type:ContactEvent")** | The Sync delegate of a certain definition to call when `Collider` ends contact with another collider. |

Fields
Collapse

## Usage

Can be used to trigger any other Component with a contact event method when a contact event happens.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [ProtoFlux:On Contact Start](https://wiki.resonite.com/ProtoFlux:On_Contact_Start "ProtoFlux:On Contact Start")
- [ProtoFlux:On Contact Stay](https://wiki.resonite.com/ProtoFlux:On_Contact_Stay "ProtoFlux:On Contact Stay")
- [ProtoFlux:On Contact End](https://wiki.resonite.com/ProtoFlux:On_Contact_End "ProtoFlux:On Contact End")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColliderEventRelay&oldid=96319](https://wiki.resonite.com/index.php?title=Component:ColliderEventRelay&oldid=96319)"

Contents