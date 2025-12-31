# Component:LaserSettings

> Source: https://wiki.resonite.com/Component:LaserSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/71/LaserSettingsComponent.png/510px-LaserSettingsComponent.png)](https://wiki.resonite.com/File:LaserSettingsComponent.png) **Laser Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LaserSettings** component is used in the [Settings](https://wiki.resonite.com/Settings "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls how fast the laser responds to your movements. Lower values will make the laser more sluggish, but better at filtering tremors. Higher values will be more responsive, but also transfer more controller shake. |
| `ModulateStartAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Angle at which the laser smoothing speed will start modulating to catch up to your movements.<br>Increasing this value will require larger movements for the laser to start catching up. |
| `ModulateEndAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Related to the modulate start angle, this indicates when the modulation will reach maximum speed. By changing the start and end angles, you can control how responsive the laser is the more you move your hand. |
| `ModulateExponent` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the response curve of the laser modulation between the start and end angles. You can use this to either make the laser respond more sluggishly at first or to start responding quickly and then tapering off. |
| `ModulateSpeedMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The laser smoothing speed will be multiplied by this value once you have reached the modulate end angle. Increasing this value will make the laser catch up quicker once you move your hand far enough. Lowering the value will make it take longer to catch up. |
| `StickThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls how much the laser will stick to interactive items. Larger values will make it stick more. Setting this to zero will stop the stickiness completely. |
| `ShowInDesktop` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When on, the laser visual will be rendered to you fully when in first person view in desktop mode. |

Fields
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LaserSettings&oldid=98947](https://wiki.resonite.com/index.php?title=Component:LaserSettings&oldid=98947)"

Contents