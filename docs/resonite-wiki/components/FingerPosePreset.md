# Component:FingerPosePreset

> Source: https://wiki.resonite.com/Component:FingerPosePreset

Collapse **Component image**

[File:FingerPosePresetComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FingerPosePresetComponent.png "File:FingerPosePresetComponent.png") **Finger Pose Preset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerPosePreset** component is itself a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent") type component that it's finger pose data is determined by the preset selected in `PresetPose`.

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PresetPose` | **[FingerPosePreset.Preset](https://wiki.resonite.com/Component:FingerPosePreset#Preset)** | The Finger pose data this component's finger pose data should be. |

Fields
Collapse

## Preset

| Name | Value | Description |
| --- | --- | --- |
| `Idle` | 0 | Hand in idle position, open relaxed. |
| `Fist` | 1 | hand balled into a fist. |
| `Point` | 2 | hand making a pointing gesture. |

Values

## Usage

Select a [Preset](https://wiki.resonite.com/Component:FingerPosePreset#Preset) for `PresetPose`. This component can now be used as a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent") in other components that mix or use such data.

## See Also

- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerPosePreset&oldid=97507](https://wiki.resonite.com/index.php?title=Component:FingerPosePreset&oldid=97507)"

Contents