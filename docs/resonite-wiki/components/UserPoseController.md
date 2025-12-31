# Component:UserPoseController

> Source: https://wiki.resonite.com/Component:UserPoseController

Collapse **Component image**

[File:UserPoseControllerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=UserPoseControllerComponent.png "File:UserPoseControllerComponent.png") **User Pose Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserPoseController** component is used to control the posing of the user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ScreenController` | **[ScreenController](https://wiki.resonite.com/Component:ScreenController "Component:ScreenController")** | the currently used screen controller. |
| `BodyHorizontalAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current user body angle. |
| `RenderDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to render the debug visuals. |
| `PauseLocomotionAnimation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to pause the current locomotion animation. |
| `OverrideLocomotionVelocity` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | What to override the current locomotion animation with. |
| `OverrideLocomotionAngularVelocity` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | What to override the current locomotion animation angular velocity with. |
| `SimulationSpeedRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The specified simulation speed ratio. |
| `_defaultConfig` | **[LocomotionAnimationConfiguration](https://wiki.resonite.com/Component:LocomotionAnimationConfiguration "Component:LocomotionAnimationConfiguration")** | What the default locomotion animation for all avatars that don't specify it should be. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserPoseController&oldid=106607](https://wiki.resonite.com/index.php?title=Component:UserPoseController&oldid=106607)"

Contents