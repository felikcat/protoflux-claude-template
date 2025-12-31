# Component:InteractionHandler

> Source: https://wiki.resonite.com/Component:InteractionHandler

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:InteractionHandler&diff=112333) which are not marked for translation.

Collapse **Component image**

[File:InteractionHandlerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InteractionHandlerComponent.png "File:InteractionHandlerComponent.png") **Interaction Handler** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Interaction Handler** component is used to control and handle the user interactions like grabbing, tooltips, and all general controls for the user regarding their hands.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Side` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | Specifies Left or Right Hand |
| `LocomotionController` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LocomotionController](https://wiki.resonite.com/Component:LocomotionController "Component:LocomotionController") >** | The locomotion controller the user is using |
| `GrabSmoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth grabbing interactions |
| `_streamDriver` | **[InteractionHandlerStreamDriver](https://wiki.resonite.com/Component:InteractionHandlerStreamDriver "Component:InteractionHandlerStreamDriver")** | The stream providing info from the user regarding interaction using hands. |
| `_undoItem` | **[ContextMenuItem](https://wiki.resonite.com/Component:ContextMenuItem "Component:ContextMenuItem")** | The context menu item used to [undo](https://wiki.resonite.com/Undo "Undo") actions for this user. |
| `_redoItem` | **[ContextMenuItem](https://wiki.resonite.com/Component:ContextMenuItem "Component:ContextMenuItem")** | The context menu item used to [redo](https://wiki.resonite.com/Undo "Undo") actions for this user. |
| `ContextMenu` | **[ContextMenu](https://wiki.resonite.com/Component:ContextMenu "Component:ContextMenu")** | The context menu for the user. |
| `EquippingEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user can equip stuff. |
| `MenuEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user can use their menu. |
| `UserScalingEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user can scale themselves. |
| `VisualEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user's visual is enabled. |
| `PointingGrab` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is grabbing with this hand via the pointer. (remote grabbing) |
| `PointingTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is physical grabbing with this hand. |
| `_toolRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the tool equipped to this hand currently. |
| `_laserSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The laser object slot of this hand. |
| `_laserPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The laser position of this hand. |
| `_laserRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The laser rotation of this hand. |
| `_interactionLaser` | **[InteractionLaser](https://wiki.resonite.com/Component:InteractionLaser "Component:InteractionLaser")** | The interaction laser component of this hand. |
| `_laserEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user's laser is enabled for this hand. |
| `_handGrabType` | **[InteractionHandler.HandGrabType](https://wiki.resonite.com/Component:InteractionHandler#HandGrabType)** | The hand grab type being used for this hand. |
| `_grabToggle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user's grabbing is enabled for this hand. |
| `_holderPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The holder position field for this hand. |
| `_holderRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The holder rotation field for this hand. |
| `_laserRotationType` | **[InteractionHandler.LaserRotationType](https://wiki.resonite.com/Component:InteractionHandler#LaserRotationType)** | The rotation type for this hand's laser. |
| `_holderAxisOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The holder axis offset for this hand. |
| `_holderRotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The holder rotation offset for this hand. used for laser rotation. |
| `_holderRotationReference` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | the reference value for the holder rotation for this hand. used for laser rotation. |
| `_originalTwistOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the original twist value for this holder. used for laser rotation. |
| `_userspaceToggleIndicator` | **[RingMesh](https://wiki.resonite.com/Component:RingMesh "Component:RingMesh")** | The |
| `ToolHolder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that holds tooltips for this hand. |
| `ShowInteractionHints` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show tooltip interaction hints for this hand for the user. |
| `_grabberSphereActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether the grab sphere visual should be visible. |
| `_grabIgnoreRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot which to ignore grabbable objects for this hand. |
| `_grabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | The grabber component for this hand to handle grabbing objects. |
| `_currentGrabType` | **[InteractionHandler.GrabType](https://wiki.resonite.com/Component:InteractionHandler#GrabType)** | The current grab type selected for this hand. |
| `ActiveToolLink` | _direct_ **[LinkTargetRef\`1](https://wiki.resonite.com/index.php?title=Type:LinkTargetRef%601&action=edit&redlink=1 "Type:LinkTargetRef`1 (page does not exist)") < [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool") >** | The link that references to the active tool for this hand. Points to the `_equipLink` on the equipped tool for this hand. |
| `_activeToolGripPoseReference` | **[GripPoseReference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference")** | The grip pose reference to use for positioning the active tool for the user in this hand. |
| `_toolLocked` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tool is equipped and locked into place. |
| `_grabMaterial` | **[FresnelMaterial](https://wiki.resonite.com/Component:FresnelMaterial "Component:FresnelMaterial")** | The material used for the grab sphere visual for this hand. |
| `_itemShelfSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot for the current item shelf on the user. |
| `_itemShelf` | **[ItemShelf](https://wiki.resonite.com/Component:ItemShelf "Component:ItemShelf")** | The component for the current item shelf on the user. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Dequip:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The button handler for dequipping a tool on this hand. |
| `EquipGrabbed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for equipping a grabbed tool on this hand. |
| `OpenLocomotionMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for opening the locomotion on this hand via the menu. |
| `OpenGrabbingMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for opening the grabbing options on this hand via the menu. |
| `OpenHandGrabMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for opening the hand grabbing options on this hand via the menu. |
| ``SetLocomotion:ButtonEventHandler`1<ILocomotionModule>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule") >** | ✓ | The handler for setting the active locomotion on this hand via the menu. |
| ``SetGrabType:ButtonEventHandler`1<InteractionHandler.HandGrabType>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [InteractionHandler.HandGrabType](https://wiki.resonite.com/Component:InteractionHandler#HandGrabType) >** | ✓ | The handler for setting the hand grab type on this hand via the menu. |
| `DestroyGrabbed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for destroying the grabbed objects on this hand via the menu. |
| `DuplicateGrabbed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for duplicating the grabbed objects on this hand via the menu. |
| `SaveGrabbed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for saving the grabbed objects on this hand via the menu. |
| `Undo:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for redoing an action via the menu on this hand. |
| `Redo:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for undoing an action via the menu on this hand. |
| `ResetUserScale:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for resetting the user's scale via the menu on this hand. |
| `OnStraighten:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for straightening the grabbed object to the closest vertical axis on this hand. |
| `OnRotateUp:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for rotating the grabbed object to the up direction on this hand, |
| `OnRotateRight:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for rotating the grabbed object to the right direction on this hand, |
| `OnRotateForward:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for rotating the grabbed object to the forward direction on this hand, |
| `OnRotateUnconstrained:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The handler for rotating the grabbed object on this hand, |

Triggers
Collapse

## HandGrabType

used when [InteractionHandler.GrabType](https://wiki.resonite.com/Component:InteractionHandler#GrabType) is set to "Hand"

| Name | Value | Description |
| --- | --- | --- |
| `Palm` | 0 | Grab via grab sphere influence. |
| `Precision` | 1 | Grab only the grabbable object which is closest to the midpoint between the index finger and the thumb of the hand. |
| `Auto` | 2 | Automatically decide whether to use "Palm" or "Precision". |
| `Off` | 3 | Hand grabbing is disabled. |

Values

## LaserRotationType

| Name | Value | Description |
| --- | --- | --- |
| `AxisX` | 0 | Rotate the grabbed item along the X axis. |
| `AxisY` | 1 | Rotate the grabbed item along the Y axis. |
| `AxisZ` | 2 | Rotate the grabbed item along the Z axis. |
| `Unconstrained` | 3 | Rotate the grabbed item along any axis. even all 3 at once. |

Values

## GrabType

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | No grabbing allowed. |
| `Hand` | 1 | Grab via hand only. |
| `Laser` | 2 | Grab via laser only. |
| `Touch` | 3 | Grab via touch only. |

Values

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Found on the right and left controller objects which are slots under the user's root slot.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractionHandler&oldid=112333](https://wiki.resonite.com/index.php?title=Component:InteractionHandler&oldid=112333)"

Contents