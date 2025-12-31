# Component:PhysicalLocomotion

> Source: https://wiki.resonite.com/Component:PhysicalLocomotion

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/52/PhysicalLocomotionComponent.png/510px-PhysicalLocomotionComponent.png)](https://wiki.resonite.com/File:PhysicalLocomotionComponent.png) **Physical Locomotion** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PhysicalLocomotion** component is a versatile [Locomotion Module](https://wiki.resonite.com/Locomotion_Modules_(Slot) "Locomotion Modules (Slot)") that can be used for walking, climbing, flying, and Zero-G.

# Fields

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
| `Archetype` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [LocomotionArchetype](https://wiki.resonite.com/Type:LocomotionArchetype "Type:LocomotionArchetype") >** | Used to specify what kind of locomotion this is, to help with identification in flux and compatibility with user settings. |
| `MinInitializationDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum time to wait for the locomotion to allow initalization. |
| `MaxInitializationDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If the amount of time passed after this component was created is past this value, the locomotion is forced to initialize anyways. |
| `InitializationColliderRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot which a collider in its hiearchy has to be raycastable (From the user's feet downward) in order for this locomotion to initalize. |
| `UseSpeedFromUserSettings` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow the speed in the user settings to influence this locomotion's speed. |
| `Description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of this locomotion in the context menu. |
| `Mode` | **[PhysicalLocomotion.MovementMode](https://wiki.resonite.com/Component:PhysicalLocomotion#MovementMode)** | How the enviroment/user influences how this locomotion can move. |
| `Gripping` | **[PhysicalLocomotion.EnvironmentGripping](https://wiki.resonite.com/Component:PhysicalLocomotion#EnvironmentGripping)** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `GripOnHold` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `GripRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `GripVelocityMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `GripHandRotationMode` | **[PhysicalLocomotion.GripRotation](https://wiki.resonite.com/Component:PhysicalLocomotion#GripRotation)** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `GripObjectRotationMode` | **[PhysicalLocomotion.GripRotation](https://wiki.resonite.com/Component:PhysicalLocomotion#GripRotation)** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `HandGripRotationSmoothSpeed` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | See [#Gripping](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping) for more information |
| `FallRespawnPosition` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far down in global space the user needs to be to respawn. |
| `MakeGravityCharacterLocal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the gravity should be based on the user's parent space orientation (true) or global (false) |
| `AutoAlignVerticalWithGravitySpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to rotate the player to orient them to the direction of gravity. |
| `ManualAlignVerticalWithGravitySpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the user aligns with gravity if 3 axis rotation is enabled and they're pressing the manual align button. |
| `AirDecelerationSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the user is slowed down while in air. |
| `GripScaleDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the user has to wait after gripping a surface in order to be able to scale with both hands in VR. |
| `AllowCrouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this locomotion allows the user to crouch down. |
| `MaximumNormalizedSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The fastest speed this locomotion is allowed to travel. |
| `_defaultIcon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The default icon url for this kind of locomotion. |
| `_defaultColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The default color for this kind of locomotion. |
| `_characterController` | **[CharacterController](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController")** | The character controller associated with this locomotion component. |
| `__legacyName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Internal. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `PresetWalkRun:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Walk run preset button is touched. |
| `PresetWalkRunGrip:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the walk run and grip preset button is touched. |
| `PresetZeroG:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the zero gravity preset button is touched. |
| `PresetPhysicalFly:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the physical fly preset button is touched. |

Triggers
Collapse

# Usage

## MovementMode

| Name | Value | Description |
| --- | --- | --- |
| `GroundTraction` | 0 | Only move when making contact with ground. |
| `DirectionalForce` | 1 | Move in the direction of the controller (VR) or head (Desktop). |

Values

## Gripping

PhysicalLocomotion has a feature which is unique to it, called Gripping. This feature allows you to grip other objects in the world in order to use them to climb or traverse the world. A good analogy is rock climbing as this is exactly how this feature feels to use. Gripping, only works when allowed by the world author.

**This feature is commonly called "Climbing" or "Physical Grab/Climbing" or even "Player Climbing", the official name "Gripping" will be used throughout this page**.

Additionally, this feature is often confused with "Grabbables" which refer to any object in that you can move around in the world by grabbing it. These features are independent, for a quick way to remember the difference:

- Grabbing involves ' _moving an object_ which you are "Grabbing"
- Gripping involves **moving you** using an object which you are "Gripping"

Or if that doesn't work, its the difference between climbing a ladder and moving that ladder.

World authors can configure this feature by changing the properties on the PhysicalLocomotion component. The main property here is "Gripping" which has the following settings and meanings:

### EnviromentGripping

| Name | Value | Description |
| --- | --- | --- |
| `Disabled` | 0 | Fully prevents any gripping in this world when using this locomotion module. |
| `GrippableObjects` | 1 | Allows gripping on objects that are explicitly tagged with a Component that indicates that a Slot or Object can be gripped. These components are: [Component:LocomotionGrip](https://wiki.resonite.com/Component:LocomotionGrip "Component:LocomotionGrip") \- The most common. Used to explicitly signal the grippable state of an object.<br>[Gizmo](https://wiki.resonite.com/Gizmo "Gizmo") \- These are also tagged as "GrippableObjects" but cannot be gripped, see [#Gripping Process](https://wiki.resonite.com/Component:PhysicalLocomotion#Gripping_Process) below for more info.<br>[Character type Colliders](https://wiki.resonite.com/Type:ColliderType "Type:ColliderType") Allows gripping on objects that contain colliders who's "CharacterCollider" property is enabled. |
| `AnyObjects` | 2 | Allows gripping on anything, including players. |

Values

### GripRotation

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | The rotation of the gripping hand does not affect user rotation/position. |
| `VerticalOnly` | 1 | The rotation of the gripping hand only affects user rotation in the vertical axis and rotates the position of the user by that offset. |
| `Any` | 2 | The rotation of the gripping hand allows the user to tilt and rotate their body using the wrist as the rotation anchor point, keeping their hand at the same position and rotation relative to the collider it is grabbing. |

Values

### Gripping Process

When a user attempts to grip in a world, the following steps occur to determine if there is a successful grip or not.

1. If gripping is set to Disabled, stop. You can't grip **ever**.
2. If there is already a grip in progress, as in is this user already holding onto another object. Stop. You can only have one active grip.
3. Run a physics operation to get any colliders within the "GripRadius" of the user's actively gripping hand.
4. Filter the returned colliders:
1. If the collider's active user is the same as the active user of the collider, remove it from the results.
2. If gripping is set to AnyObjects, all colliders in the "GripRadius" are included.
3. If gripping is set to CharacterColliders, colliders who do **NOT** have the "CharacterCollider" checkbox enabled are removed from the results.
4. If gripping is set to GrippableObjects, colliders who do **NOT** have a "LocomotionGrip" component on them or within their parents are removed from the results.
5. From the filtered list the **first** collider which passes **ALL** the following rules is then "Gripped":

1. If the collider has a "LocomotionGrip" component on them or within their parents, it must be Enabled.
2. The collider must **NOT** be a part of a Gizmo

### Gripping Users

Gripping users is treated the same way as the "Gripping Process" above. So keep the following items in mind:

- You cannot manually **opt in** to be grippable by editing your avatar **unless the Gripping property on the locomotion is set to "GrippableObjects"**, if this is the case add a "LocomotionGrip" component to your avatar root and enable it.
- If you want to **opt out** of being grippable then regardless of the world settings, you will need to add a "LocomotionGrip" component to your **avatar root AND User Root** and uncheck their Enabled properties.

# Examples

Is part of the default world locomotion set using the walk locomotion.

# See Also

- [Other locomotion module types](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PhysicalLocomotion&oldid=99088](https://wiki.resonite.com/index.php?title=Component:PhysicalLocomotion&oldid=99088)"

Contents