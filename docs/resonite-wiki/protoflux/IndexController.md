# ProtoFlux:IndexController

> Source: https://wiki.resonite.com/ProtoFlux:IndexController

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Index Controller

User

IsActive

Node

Type

BatteryLevel

BatteryCharging

ButtonA

ButtonB

ButtonA\_Touch

ButtonB\_Touch

Grip

GripTouch

GripClick

Joystick

JoystickTouch

JoystickClick

Trigger

TriggerTouch

TriggerClick

Touchpad

TouchpadTouch

TouchpadPress

TouchpadForce

Controllers

This node provides information provided by Index controllers.

## Inputs

### User ( [User](https://wiki.resonite.com/User "User"))

The user to get controller information from.

### Node ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The controller side to get information from.

## Outputs

### IsActive ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Bool for showing if the device is active. Useful for troubleshooting if your controller is not responding.

### Type ( [Type](https://wiki.resonite.com/Type:Type "Type:Type"))

The controller type being used. (type of [IndexController](https://wiki.resonite.com/index.php?title=Type:IndexController&action=edit&redlink=1 "Type:IndexController (page does not exist)") if exists or `null`)

### BatteryLevel ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The battery level of this controller. (`1`: full, `0`: empty)

### BatteryCharging ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the battery is currently charging.

### ButtonA ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the A button is being pressed.

### ButtonB ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the B button is being pressed.

### ButtonA\_Touch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the capacitive touch is being pressed on A button.

### ButtonB\_Touch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the capacitive touch is being pressed on B button.

### Grip ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

Shows the strength of the grip on the device. (from `0` to `1`)

### GripTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the grip is being touched.

### GripClick ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the grip is being gripped enough to trigger a grab action.

### Joystick ( [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The position of this controller's joystick. (`[-1; -1]`: backward left, `[+1; +1]`: forward right, `[0; 0]`: resting position)

### JoystickTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the controller's joystick being touched right now.

### JoystickClick ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the controller's joystick clicked down right now.

### Trigger ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

Shows the strength of the trigger while pressed. (from `0` to `1`)

### TriggerTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the trigger is being touched.

### TriggerClick ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the trigger is pushed enough to trigger a click action.

### Touchpad ( [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Shows the X and Y of the area where the Touchpad is touched. (`[-1; -1]`: bottom left, `[+1; +1]`: top right, `[0; 0]` when untouched)

### TouchpadTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the touchpad being touched.

### TouchpadPress ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the touchpad being touched enough to trigger a click action.

### TouchpadForce ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

Shows the strength of the touch on the touchpad. (from `0` to `1`)

## Examples

### Driving a blendshape with a button press

Controller nodes are commonly used to create gesture systems, where pressing a button or combination of buttons can control a blendshape, which usually are 'emotes' on avatars with custom facial expressions.

- To define whose controller will be used in the node, you must input the User. Using the [Get Active User Self](https://wiki.resonite.com/ProtoFlux:Get_Active_User_Self "ProtoFlux:Get Active User Self") node will ensure that it will always be the user of the avatar, if the flux is [packed](https://wiki.resonite.com/ProtoFlux_Tool#Packing_ProtoFlux_nodes "ProtoFlux Tool") under the avatar.
- The node input also must be input which can be Left or Right.
- While many of the outputs are [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"), they can be easily changed to [Float](https://wiki.resonite.com/Type:Float "Type:Float") type by using a [ZeroOne](https://wiki.resonite.com/ProtoFlux:Zero_One "ProtoFlux:Zero One") node to translate the bool to a float.
- Getting the drive node from a blendshape, we can use that to connect to the ZeroOne node, which will 'drive' the blendshape from 0 to 1 while the button is held.

There is more detailed information on how to do this on the [Gestures](https://wiki.resonite.com/Gestures "Gestures") page.

[![](https://wiki.resonite.com/images/thumb/1/16/Indexcontroller_to_float.jpg/800px-Indexcontroller_to_float.jpg)](https://wiki.resonite.com/File:Indexcontroller_to_float.jpg) This is an example circuit of using an A button press to control a blendshape.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IndexController&oldid=110049](https://wiki.resonite.com/index.php?title=ProtoFlux:IndexController&oldid=110049)"

Contents