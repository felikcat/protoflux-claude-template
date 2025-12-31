# Component:PointTouchSource

> Source: https://wiki.resonite.com/Component:PointTouchSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a9/PointTouchSourceComponent.png/510px-PointTouchSourceComponent.png)](https://wiki.resonite.com/File:PointTouchSourceComponent.png) **Point Touch Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A simpler version of [Component:TipTouchSource](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource").

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
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of where the tip touch sources touch effects start from the slot this component is on. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction in which to interact with touchable elements using this component. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the maximum distance before hovering doesn't register |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:TipTouchSource](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PointTouchSource&oldid=106296](https://wiki.resonite.com/index.php?title=Component:PointTouchSource&oldid=106296)"

Contents