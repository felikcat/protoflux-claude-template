# Component:AudioFilterBlendWrapper

> Source: https://wiki.resonite.com/Component:AudioFilterBlendWrapper

Collapse **Component image**

[File:AudioFilterBlendWrapperComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=AudioFilterBlendWrapperComponent.png "File:AudioFilterBlendWrapperComponent.png") **Audio Filter Blend Wrapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Audio Filter Blend Wrapper** component is used to wrap other filters and provides blending functionality. This is useful for audio reverb zones, allowing each listener with its own blend weight to share the same instance of AudioZitaReverb (and potentially other filters in the future)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BlendWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of weight this filter has with other filters. |
| `NestedFilter` | **[AudioDSP\_Effect](https://wiki.resonite.com/Type:AudioDSP_Effect "Type:AudioDSP Effect")** | The filter this wraps around. |

Fields
Collapse

## Usage

See [Component:AudioListener](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener").

## Examples

See [Component:AudioListener](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener").

## See Also

- [Component:AudioListener](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener")
- [Awwdio](https://wiki.resonite.com/Awwdio "Awwdio")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioFilterBlendWrapper&oldid=101101](https://wiki.resonite.com/index.php?title=Component:AudioFilterBlendWrapper&oldid=101101)"

Contents