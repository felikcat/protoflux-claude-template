# ProtoFlux:TouchController

> Source: https://wiki.resonite.com/ProtoFlux:TouchController

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Touch Controller

User

IsActive

Node

Type

BatteryLevel

IsBatteryCharging

Model

Start

ButtonYB

ButtonXA

ButtonYB\_Touch

ButtonXA\_Touch

ThumbRestTouch

Grip

GripClick

Joystick

JoystickTouch

JoystickClick

Trigger

TriggerTouch

TriggerClick

Controllers

This node provides information provided by Meta controllers.

## Usage

You can input a [user](https://wiki.resonite.com/Type:User "Type:User") reference and a [chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality") to read the status and inputs of a user's controller.

## Inputs

### User ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user to receive inputs from.

### Node ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The side to receive inputs from.

## Outputs

### IsActive ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Bool for showing if the device is active. Useful for troubleshooting if your controller is not responding.

### Type ( [Type](https://wiki.resonite.com/Type:Type "Type:Type"))

The controller type being used.

### BatteryLevel ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

Shows the battery level of the device from 1 to 0.

### BatteryCharging ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the battery is currently charging.

### Model ( [Model](https://wiki.resonite.com/Type:Model "Type:Model"))

The controller model.

### Start ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the start button being pressed right now.

### ButtonYB ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if Y/B is being pressed.

### ButtonXA ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if X/A is being pressed.

### ButtonYB\_Touch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if Y/B is being touched.

### ButtonXA\_Touch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if X/A is being touched.

### ThumbRestTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the thumb rest is being touched.

### Grip ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

Shows a 0 to 1 value of the grip strength.

### GripClick ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if grip is being clicked.

### Joystick ( [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Gives a 2D vector of the joystick input.

### JoystickTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the joystick is being touched.

### JoystickClick ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the controller's joystick clicked down right now.

### Trigger ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The amount of how far this controller's trigger is being pressed down currently.

### TriggerTouch ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the controller's trigger being touched right now.

### TriggerClick ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Is the controller's trigger being clicked down right now.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TouchController&oldid=110865](https://wiki.resonite.com/index.php?title=ProtoFlux:TouchController&oldid=110865)"

Contents