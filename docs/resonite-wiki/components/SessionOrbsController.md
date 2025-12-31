# Component:SessionOrbsController

> Source: https://wiki.resonite.com/Component:SessionOrbsController

(Redirected from [Component:SessionOrbsController](https://wiki.resonite.com/index.php?title=Component:SessionOrbsController&redirect=no "Component:SessionOrbsController"))

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LegacySessionOrbsController&diff=99004) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e9/SessionOrbsControllerComponent.png/510px-SessionOrbsControllerComponent.png)](https://wiki.resonite.com/File:SessionOrbsControllerComponent.png) **Legacy Session Orbs Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacySessionOrbsController** component displays session orbs of current [sessions](https://wiki.resonite.com/Session "Session") into a slot. This component was used in what some players called the "Session plate" which would have many world orbs of active sessions.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

For an up-to-date counterpart, see [Component:WorldsDataFeed](https://wiki.resonite.com/Component:WorldsDataFeed "Component:WorldsDataFeed") and read on the concept [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds").


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SpawnRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of spawning orbs in a cylinder shape. |
| `SpawnHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of spawning orbs in a cylinder shape. |
| `SpawnOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of the spawn cylinder shape in local space vs the center on `_root` |
| `_root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to place and spawn session orbs. |
| `MaxOrbs` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many orbs can be under `_root` at any one time. |
| `ShowHeadless` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show headless sessions |

Fields
Collapse

## Usage

Used in items that display current sessions in Resonite.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacySessionOrbsController&oldid=99004](https://wiki.resonite.com/index.php?title=Component:LegacySessionOrbsController&oldid=99004)"

Contents