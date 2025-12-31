# Component:LocomotionController

> Source: https://wiki.resonite.com/Component:LocomotionController

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f3/LocomotionControllerComponent.png/510px-LocomotionControllerComponent.png)](https://wiki.resonite.com/File:LocomotionControllerComponent.png) **Locomotion Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocomotionController** component is used on user root slots to allow user inputs to control Locomotion modules and switch between them. It also handles disabling them when they should be restrained.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ScalingEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is allowed to scale or not. |
| `SupressSources` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Component](https://wiki.resonite.com/Type:Component "Type:Component")** | Sources of Locomotion suppression. This will usually be a [AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor"). |
| `InputSupressSources` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Component](https://wiki.resonite.com/Type:Component "Type:Component")** | A list of Components that act as input control supressors. |
| `LocomotionModules` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")** | A list of locomotions the user can switch between and use. |
| `ActiveModuleIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The current locomotion module being used. |
| `FindUserPreferredModule` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to automatically use the user's preferred locomotion in [Settings](https://wiki.resonite.com/Settings "Settings"). |
| `_currentGroundCollider` | **[ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider")** | the current object that the user is standing on (supporting ground or slope) |
| `_lastGroundCollider` | **[ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider")** | The previous collider the user was standing on before they started nocliping or otherwise. |
| `OnInitialized` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <LocomotionController>** | A sync delegate to call and pass this locomotion controller as a reference to when this component Initializes. |
| `_parentHierarchy` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | A list of slots that are parents of this component. |
| `_dummyCharacterController` | **[CharacterController](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController")** | The character controller to use when there is no locomotion. Is found on User root. |

Fields
Collapse

## Usage

Used internally by user systems made in a user slot on spawn.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionController&oldid=105304](https://wiki.resonite.com/index.php?title=Component:LocomotionController&oldid=105304)"

Contents