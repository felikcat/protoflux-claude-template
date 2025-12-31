# Component:MovementSettings

> Source: https://wiki.resonite.com/Component:MovementSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9e/MovementSettingsComponent.png/510px-MovementSettingsComponent.png)](https://wiki.resonite.com/File:MovementSettingsComponent.png) **Movement Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LeftSidewaysMode` | **[SidewaysMovementMode](https://wiki.resonite.com/Type:SidewaysMovementMode "Type:SidewaysMovementMode")** | How the left controller should be used to move the user. |
| `RightSidewaysMode` | **[SidewaysMovementMode](https://wiki.resonite.com/Type:SidewaysMovementMode "Type:SidewaysMovementMode")** | How the right controller should be used to move the user. |
| `UseHeadDirectionForMovement` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should head direction or controller direction in VR for movement direction. |
| `UseSmoothTurn` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether smooth turning using joystick should be used. |
| `SmoothTurnExclusiveMode` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use only smooth turning in all cases. |
| `SmoothTurnSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smooth turn speed sensitivity. |
| `SnapTurnAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many degrees to change by when using snap turn mode. |
| `NoClipSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the user's noclip speed should be. |
| `MovementDeadzone` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Any 0 to 1 value less than this is ignored for movement. (this is 0 to 1 range) |
| `TurningDeadzone` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Any 0 to 1 value less than this is ignored for turning.(this is 0 to 1 range) |
| `MovementExponent` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Pushes values from a 0 to 1 linear value to a quick ramp up effect still within a 0 to 1 range for movement speed input on the joysticks. |

Fields
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

See [Settings](https://wiki.resonite.com/Settings "Settings").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MovementSettings&oldid=105336](https://wiki.resonite.com/index.php?title=Component:MovementSettings&oldid=105336)"

Contents