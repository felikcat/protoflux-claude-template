# ProtoFlux:StandardController

> Source: https://wiki.resonite.com/ProtoFlux:StandardController

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Standard Controller

User

IsActive

Node

Type

BatteryLevel

IsBatteryCharging

Primary

Secondary

Grab

Menu

Strength

Axis

Controllers

This node provides information for generic controllers.

## Usage

The standard controller node allows one to interact with the players virtual reality controller as well as generic inputs on Desktop mode.

Say you want to get the user's grip and trigger strength, just feed it a user and a "Chirality input" for the left or right controller and volla!

Just pull an output from the grip boolean and the strength float value and now you have the users grip and trigger on/off and strength!

## Examples

## Inputs

### User ( [User](https://wiki.resonite.com/User "User"))

The user to get controller information from.

### Node ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The controller side to get information from.

## Outputs

### IsActive ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is this controller actively being used right now.

### Type ( [Type](https://wiki.resonite.com/Type:Type "Type:Type"))

The controller type being used. (a subtype of [IStandardController](https://wiki.resonite.com/index.php?title=Type:IStandardController&action=edit&redlink=1 "Type:IStandardController (page does not exist)") if a controller exists or `null`)

### BatteryLevel ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The battery level of this controller. (`1`: full, `0`: empty, `-1`: battery level not available)

### IsBatteryCharging ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is this controller currently charging.

### Primary ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is primary pressed right now.

### Secondary ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is secondary pressed right now.

### Grab ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the controller's grip button pressed right now.

### Menu ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the menu button being pressed right now.

### Strength ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How much the trigger is pressed currently. (from `0` to `1`)

### Axis ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The position of this controller's joystick or touchpad depending on controller type. (`[-1; -1]`: bottom left, `[+1; +1]`: top right, `[0; 0]` for touchpads that are untouched)

[Index Controllers](https://wiki.resonite.com/ProtoFlux:Index_Controller "ProtoFlux:Index Controller") have both types of input. `Axis` returns the touchpad position.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:StandardController&oldid=113161](https://wiki.resonite.com/index.php?title=ProtoFlux:StandardController&oldid=113161)"

Contents