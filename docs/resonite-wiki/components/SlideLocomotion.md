# Component:SlideLocomotion

> Source: https://wiki.resonite.com/Component:SlideLocomotion

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c4/SlideLocomotionComponent.png/510px-SlideLocomotionComponent.png)](https://wiki.resonite.com/File:SlideLocomotionComponent.png) **Slide Locomotion** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SlideLocomotion** component acts the same as a [Component:NoclipLocomotion](https://wiki.resonite.com/Component:NoclipLocomotion "Component:NoclipLocomotion") except that this locomotion will attach the user to a raycasted surface below them regardless of collider type. When a surface is not found, Behavior compared to noclip is identical.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Icon` | **[IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") >** | The icon image visual for this locomotion in the context menu. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this locomotion's icon in the context menu. |
| `_currentController` | **[LocomotionController](https://wiki.resonite.com/Component:LocomotionController "Component:LocomotionController")** | The current Locomotion controller which would be from a user controlling this locmotion. |
| `_lastDefaultIcon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The last URI used for the default context menu icon for this locomotion. |
| `_lastDefaultColor` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The last color used for the default version of this locomotion for the context menu. |
| `Turn` | _direct_ **[TurnSubmodule](https://wiki.resonite.com/index.php?title=Type:TurnSubmodule&action=edit&redlink=1 "Type:TurnSubmodule (page does not exist)")** | How turning should be handled for this locomotion. |
| `MaxSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The fastest speed this locomotion can travel. |
| `MinimumFlySpeedRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Unused. |
| `MaxSnapDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum distance to check from the user's feet position plus `SnapCheckOffset` downward. |
| `SnapCheckOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | anything from the user's feet within this range downward is not raycasted. |
| `SnapMinObjectSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum size of the object's max dimensions on any axis in global space compared to the user's max size on any axis needed for us to snap to it's surface below us. |

Fields
Collapse

## Usage

Can be used for sticky fly locomotion.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Other locomotion module types](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SlideLocomotion&oldid=95230](https://wiki.resonite.com/index.php?title=Component:SlideLocomotion&oldid=95230)"

Contents