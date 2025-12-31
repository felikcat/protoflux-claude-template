# Component:PhysicalButton

> Source: https://wiki.resonite.com/Component:PhysicalButton

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PhysicalButton&diff=94820) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3f/PhysicalButtonComponent.png/510px-PhysicalButtonComponent.png)](https://wiki.resonite.com/File:PhysicalButtonComponent.png) **Physical Button** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PhysicalButton** component can be used to create buttons that move inward when pressed by a user, a press depth and threshold can be set to customize the physical feeling of the button.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PressAxis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction in local space to go when pressing the button |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this button can only be pressed if the user is in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") |
| `ActiveUserFilter` | **[ActiveUserHandling](https://wiki.resonite.com/Type:ActiveUserHandling "Type:ActiveUserHandling")** | How to filter in or out the active user of this component. |
| `__legacyActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the legacy active user root only option. |
| `Pressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | A sync delegate to call when the button is pressed. |
| `Pressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | A sync delegate to call when the button is being pressed. is called every game update while the button is held down. |
| `Released` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | A sync delegate to call when the button is released. |
| `PressDepth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The max distance the button can move in `PressAxis` direction |
| `PressThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If pressed more than this amount, the button is considered pressed. |
| `ReleaseThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If pressed less than this amount, the button is considered released. |
| `IsPressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user has the button pressed. |
| `IsHovering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is hovering their interaction source at the button (laser or tip touch source) |
| `IsHolding` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is holding the button. |
| `IsPressedOrHolding` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the button is being held down or being pressed. |
| `Hold` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the button can be held down. |
| `HoldDepthRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the button has to be pressed before it is considered being held down. |
| `BeginPressVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate a user's hand when they begin to press the button. |
| `PressVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate a user's hand when they press the button. |
| `HoverVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate a user's hand when they point at the button. |
| `Label` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to drive with a label describing this button. |
| `_currentPressingDepth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current amount that the button is being pushed down. |
| `_buttonOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The initial position of the button's transforms in local space. |
| `_buttonPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the field to drive to influence the position of the button for pressing. |

Fields
Collapse

## Usage

Attach to a slot under another slot. the slot hiearchy this is on should have a collider in order to be able to press the button. Hooking this up to [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"), or using the [Button Events](https://wiki.resonite.com/Button_Events "Button Events") this generates will give this button functionality.

## Miscellaneous Notes

When adding this component to an object that has the [Grabbable component](https://wiki.resonite.com/Grabbable_(Component) "Grabbable (Component)"), you will notice that the object may not be grabbable anymore. To remedy this, create a child object on the main object you want to be your button. Then, on that child object, attach this component. You should now have an object that is grabbable and functions as a button.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PhysicalButton&oldid=94820](https://wiki.resonite.com/index.php?title=Component:PhysicalButton&oldid=94820)"

Contents