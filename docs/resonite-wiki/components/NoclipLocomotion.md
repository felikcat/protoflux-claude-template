# Component:NoclipLocomotion

> Source: https://wiki.resonite.com/Component:NoclipLocomotion

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/05/NoclipLocomotionComponent.png/510px-NoclipLocomotionComponent.png)](https://wiki.resonite.com/File:NoclipLocomotionComponent.png) **No clip Locomotion** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NoclipLocomotion** component when being used as an active locomotion by the user allows for a user to go through walls.

If all of a user's colliders on their avatar are set up with their [Component:VRIKAvatar](https://wiki.resonite.com/Component:VRIKAvatar "Component:VRIKAvatar")'s collider list, they won't trigger any trigger zones during noclip.

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
| `MaxSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the user can go in this mode. |
| `MinimumFlySpeedRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Unused. |

Fields
Collapse

## Usage

When attached to a slot, the component will add the nessary complementary components in order for it to function. When placed under the world lomotions slot, it will be added to every new user's locomotion menu.

This can also be injected into a user using locomotion injector [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

## Examples

Used in the default provided world locomotion.

## See Also

- [Other locomotion module types](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NoclipLocomotion&oldid=95226](https://wiki.resonite.com/index.php?title=Component:NoclipLocomotion&oldid=95226)"

Contents