# Component:RelayTouchSource

> Source: https://wiki.resonite.com/Component:RelayTouchSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c9/RelayTouchSourceComponent.png/510px-RelayTouchSourceComponent.png)](https://wiki.resonite.com/File:RelayTouchSourceComponent.png) **Relay Touch Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RelayTouchSource** component is used to handle the interactions of tip touch sources on the user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoUpdateUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user handling updates for thus component |
| `OutOfSightAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Buttons outside this angle from the user's center view are considered out of sight. |
| `MaxTouchPenetrationDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The max distance of penetration into an item like a physical button before it's not considered pressed anymore. |
| `TipPositionGetter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") <RelayTouchSource, [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Refers to a [InteractionLaser](https://wiki.resonite.com/Component:InteractionLaser "Component:InteractionLaser")'s sync delegate of the same name. |
| `TipDirectionGetter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") <RelayTouchSource, [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | Refers to a [InteractionLaser](https://wiki.resonite.com/Component:InteractionLaser "Component:InteractionLaser")'s sync delegate of the same name. |
| `TouchTypeGetter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") <RelayTouchSource, [TouchType](https://wiki.resonite.com/Type:TouchType "Type:TouchType") >** | Refers to a [InteractionLaser](https://wiki.resonite.com/Component:InteractionLaser "Component:InteractionLaser")'s sync delegate of the same name. |
| `TouchableGetter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[TouchableGetter](https://wiki.resonite.com/index.php?title=Type:TouchableGetter&action=edit&redlink=1 "Type:TouchableGetter (page does not exist)")** | Refers to a [InteractionLaser](https://wiki.resonite.com/Component:InteractionLaser "Component:InteractionLaser")'s sync delegate of the same name. |

Fields
Collapse

## Usage

Not usually used by the user. However, a [TipTouchSource](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") component is.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RelayTouchSource&oldid=98928](https://wiki.resonite.com/index.php?title=Component:RelayTouchSource&oldid=98928)"

Contents