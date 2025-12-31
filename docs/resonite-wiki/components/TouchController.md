# Component:TouchController

> Source: https://wiki.resonite.com/Component:TouchController

Describes general HMD controller.

## Input

- User: [User](https://wiki.resonite.com/Type:User "Type:User"): Equipee of the controller. should not be null.
- Node: [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"): The side of the controller. should not be null.

## Output

- IsActive: [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"): is controller active?
- Type: [Type](https://wiki.resonite.com/Type:Type "Type:Type"): The internal class for handling device I/O. Defaults to null.
- BatteryLevel: [Float](https://wiki.resonite.com/Type:Float "Type:Float"): How its battery is charged? Default to -1 if it cannot be retrieved.
- IsBatteryCharging: Bool
- Model: [Model](https://wiki.resonite.com/Type:Model "Type:Model")
- Start: Bool
- ButtonYB: Bool: are they pressed?
- ButtonXA: Bool: are they pressed?
- ButtonYB\_Touch: are they touched?
- ButtonXA\_Touch: are they touched?
- ThumbRestTouch: are there touched input key where touchable by thumb other than buttons and joysticks? (Requires verification: does this include joystick touch?)
- Grip: Float: press strength of grip. Between 0 (not gripped) and 1 (completely gripped).
- GripClick: Bool: is grip pressed?
- Joystick: [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"): reports rotation amount by each axis.
- JoystickTouch: Bool: is joystick touched?
- JoystickClick: Bool: is joystick clicked down?
- Trigger: Float: press strength of trigger. Same as Grip.
- TriggerTouch: Bool: is trigger touched?
- TriggerClick: Bool: is trigger clicked?

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchController&oldid=80554](https://wiki.resonite.com/index.php?title=Component:TouchController&oldid=80554)"

Contents