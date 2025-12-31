# Component:TipTouchSource

> Source: https://wiki.resonite.com/Component:TipTouchSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7c/TipTouchSourceComponent.png/510px-TipTouchSourceComponent.png)](https://wiki.resonite.com/File:TipTouchSourceComponent.png) **Tip Touch Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TipTouchSource** component is responsible for interaction with touchable objects like buttons and touch buttons. This component gains functionality after being activated by a [Component:AvatarHandDataAssigner](https://wiki.resonite.com/Component:AvatarHandDataAssigner "Component:AvatarHandDataAssigner") upon avatar equip.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoUpdateUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | which user should be updating this component's logic. Defaults to active user if not filled. |
| `OutOfSightAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | disables the function of this component if the updating user is looking more than this many degrees away from this component's slot. |
| `MaxTouchPenetrationDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far it can go into the touchable's collider before its not considered as touching. |
| `CustomFilter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | similar to [UVRaycastPortal's](https://wiki.resonite.com/Component:MeshUVRaycastPortal "Component:MeshUVRaycastPortal")`Filter` field. Internal. |
| `UseUserSpaceForDistance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to use local space for distance or use absolute world distance for distance. |
| `TouchDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how far in meters that this can touch things |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum distance before hovering doesn't register |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the offset for everything this component does from the slot this component is on. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction this can touch things. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used on the index finger of user hands so that it can physically press buttons.

## See Also

- [Component:PointTouchSource](https://wiki.resonite.com/Component:PointTouchSource "Component:PointTouchSource")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TipTouchSource&oldid=95416](https://wiki.resonite.com/index.php?title=Component:TipTouchSource&oldid=95416)"

Contents