# Component:GrabWorldLocomotion

> Source: https://wiki.resonite.com/Component:GrabWorldLocomotion

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b0/GrabWorldLocomotionComponent.png/510px-GrabWorldLocomotionComponent.png)](https://wiki.resonite.com/File:GrabWorldLocomotionComponent.png) **Grab World Locomotion** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabWorldLocomotion** component can be used to make a locomotion for a world or injected into a user from an avatar or tooltip.

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
| `ActivationThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The primary strength from the user before activation. |
| `DeactivationThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The primary strength from the user before deactivation. |
| `_visual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot of the cross mesh visual used when moving. |
| `_crossMesh` | **[CrossMesh](https://wiki.resonite.com/Component:CrossMesh "Component:CrossMesh")** | The cross mesh that should appear at the user's hand whenever moving with this locomotion. |
| `_material` | **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material applied to the cross mesh visual. |

Fields
Collapse

## Usage

Can be used by making this locomotion active via the context menu. When used as a locomotion, it can allow for fine turning by pressing left and right and fine translational precision control by pressing forward on the joystick.

## Examples

Can be used for small movement maneuvering where precision is key.

## See Also

- [Other locomotion module types](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabWorldLocomotion&oldid=95228](https://wiki.resonite.com/index.php?title=Component:GrabWorldLocomotion&oldid=95228)"

Contents