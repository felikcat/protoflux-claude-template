# Component:DroneCamera

> Source: https://wiki.resonite.com/Component:DroneCamera

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3a/DroneCameraComponent.png/510px-DroneCameraComponent.png)](https://wiki.resonite.com/File:DroneCameraComponent.png) **Drone Camera** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DroneCamera** is a component commonly used in 3rd person free cam desktop. It can also be influenced via [Command Line Arguments](https://wiki.resonite.com/Command_Line_Arguments "Command Line Arguments") to change it's behavior.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CameraUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that should be simulating this camera. |
| `SimulateOnHost` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to simulate the camera on the host. |
| `ManualControl` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is manually controlling the camera. |
| `SlowSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | meters per second to move when going slow. |
| `Speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Meters per second when going normal speed. |
| `FastSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | meters per second when holding shift. |
| `MouseSensitivity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The look speed sensitivity. |
| `FieldOfViewSource` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to use as the field of view value. |
| `FieldOfView` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field of view in absence of a value for `FieldOfViewSource`. |
| `AspectRatioSource` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to use as the aspect ratio source. |
| `AspectRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The aspect ratio in absence of a value for `AspectRatioSource`. |
| `FollowUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user to follow. |
| `ControllerRejectDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Distance limit for rejecting a controller. |
| `GroupSearchRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius to search for groups of users. |
| `BiggestGroupSearchInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The time to wait before checking for the largest group of users in the world to track. |
| `IgnoreOtherCameras` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to ignore other cameras. |
| `HeadForwardPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from a user's head in a group to stay back from when the camera in front of them. |
| `HeadBackwardPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from a user's head in a group to stay back from when the camera is behind them. |
| `HeadUpPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from a user's head in a group to stay back from when the camera is above them. |
| `HeadDownPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from a user's head in a group to stay back from when the camera is below them. |
| `HeightOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far up or down to look from a target user's view point. |
| `CircleOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The offset from the circle around a user to position this component |
| `DistanceOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance offset to have from a target. |
| `CircleSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to travel a circle around a target. |
| `PositionSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed of this component's position change. |
| `LookSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The look around speed of the camera. |
| `DistanceSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to close the distance in seconds to a target position when focusing on something or a UI. |
| `UserInfluenceSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to restore user influence. |
| `HeightAmplitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height Amplitude for a target height. |
| `DistanceAmplitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance Amplitude for a target distance from a subject. |
| `CircleAmplitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The circle Amplitude for a circle distance. |
| `HeightPeriod` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The period in which to change height. |
| `DistancePeriod` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The period in which to change distance. |
| `CirclePeriod` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The period in which to change circle distance. |
| `CirclePeriodNoiseSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed of noise influence on the circle period attribute. |
| `CirclePeriodNoiseInfluence` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The influence of noise on the circle period attribute. |
| `CheckOcclusion` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to check if a subject has parts of them occluded. |
| `AdjustHeightOnOcclusion` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to adjust camera height when the target is occluded. |
| `TeleportWaitTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long to wait before teleporting to a target position. |
| `TeleportTriggerRelativeDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far of a distance is needed to teleport to a target position. |
| `TeleportTriggerAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big of an angle needed to teleport to a target rotation. |
| `MinRandomizeFovInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum time to wait before randomly changing the camera FOV. |
| `MaxRandomizeFovInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum time to wait before randomly changing the camera FOV. |
| `MinFov` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum FOV this camera can randomly change to. |
| `MaxFov` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum FOV this camera can randomly change to. |
| `MinChangeFovTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum time it takes for the FOV on this camera to change randomly. |
| `MaxChangeFovTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum time it takes for the FOV on this camera to change randomly. |

Fields
Collapse

## Usage

Used in free cam mode or to follow groups.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DroneCamera&oldid=96454](https://wiki.resonite.com/index.php?title=Component:DroneCamera&oldid=96454)"

Contents