# Component:TeleportLocomotion

> Source: https://wiki.resonite.com/Component:TeleportLocomotion

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/TeleportLocomotionComponent.png/510px-TeleportLocomotionComponent.png)](https://wiki.resonite.com/File:TeleportLocomotionComponent.png) **Teleport Locomotion** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TeleportLocomotion** component is used to allow users to teleport to spots using an arc path as a location selector.

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
| `BackstepDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far to go backwards when pressing the backwards movement direction. |
| `ActivationTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long it takes for the teleport visual to show and for the locomotion to allow teleport when pressing the forward movement direction. |
| `HeightInputMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum teleport up distance. |
| `HeightInputMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum teleport height distance. |
| `InitialForceMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum inital arc force value for the destination selection arc. |
| `InitialForceMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum inital arc force value for the destination selection arc. |
| `RangeExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to boost the teleport range. |
| `StepUnit` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What to use for the step value in the teleport arc. |
| `Drag` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What to use for the drag value in the teleport arc. |
| `MaxSmallObjectSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum size to allow before a small object is not ignored for teleport destinations. |
| `WallDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The depth a wall has to be compared to the user's size to be considered a wall. |
| `_pathMesh` | **[BallisticPathMesh](https://wiki.resonite.com/Component:BallisticPathMesh "Component:BallisticPathMesh")** | The path mesh being used to display this locomotion's teleport location selector. |
| `_pathMaterial` | **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material to control the look of that is on `_pathMesh`. |
| `_pathRenderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The renderer of this teleport locomotion's location selector visual. |
| `_pathVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root slot of this teleport locomotion's location selector visual |
| `_targetPointVisual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root of the hit point visual of this teleport locomotion's location selector visual |
| `_characterController` | **[CharacterController](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController")** | The character controller for this teleport locomotion. |

Fields
Collapse

## Usage

Used for accessibility reasons, and for puzzle games.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Other locomotion module types](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TeleportLocomotion&oldid=95231](https://wiki.resonite.com/index.php?title=Component:TeleportLocomotion&oldid=95231)"

Contents