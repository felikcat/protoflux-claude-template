# Component:EarmuffSettings

> Source: https://wiki.resonite.com/Component:EarmuffSettings

Collapse **Component image**

[File:EarmuffSettingsComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=EarmuffSettingsComponent.png "File:EarmuffSettingsComponent.png") **Earmuff Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **EarmuffSettings** component is used to allow a user to change the settings for the Ear muffs, which reduce the noise outside of a cone emitted from the user's head. This feature is useful in crowds or noisy places

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EarmuffEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to have the earmuffs mode enabled for the local user |
| `VolumeAttenuation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to reduce volume based on its distance from the cone. |
| `Directionality` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the audio is affected by how in front the audio is. |
| `Distance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far forward from the user's head the cone should stretch |
| `Angle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle of the cone. |
| `TransitionStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The start of audio reducing outside the cone. |
| `TransitionLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance outside the cone that audio becomes quiet over distance from the cone. |

Fields
Collapse

## Usage

Is used for the settings earmuffs. Is not used directly by the user.

## Examples

Used in the settings tab in the dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EarmuffSettings&oldid=96460](https://wiki.resonite.com/index.php?title=Component:EarmuffSettings&oldid=96460)"

Contents