# Component:AudioTypeGroupVolumeSlider

> Source: https://wiki.resonite.com/Component:AudioTypeGroupVolumeSlider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/AudioTypeGroupVolumeSliderComponent.png/510px-AudioTypeGroupVolumeSliderComponent.png)](https://wiki.resonite.com/File:AudioTypeGroupVolumeSliderComponent.png) **AudioTypeGroupVolumeSlider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioTypeGroupVolumeSlider** component is used in [userspace](https://wiki.resonite.com/Userspace "Userspace") for volume sliders, specifically for the different volume groups.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Slider` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The slider that is changing the audio. |
| `Group` | **[AudioTypeGroup](https://wiki.resonite.com/Type:AudioTypeGroup "Type:AudioTypeGroup")** | The audio type to change the audio for. |

Fields
Collapse

## Usage

## Examples

Used in [userspace](https://wiki.resonite.com/Userspace "Userspace") for volume sliders, specifically for the different volume groups.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioTypeGroupVolumeSlider&oldid=100122](https://wiki.resonite.com/index.php?title=Component:AudioTypeGroupVolumeSlider&oldid=100122)"

Contents