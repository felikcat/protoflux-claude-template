# Component:LocalLightsBufferRenderer

> Source: https://wiki.resonite.com/Component:LocalLightsBufferRenderer

Collapse **Component image**

[File:LocalLightsBufferRendererComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LocalLightsBufferRendererComponent.png "File:LocalLightsBufferRendererComponent.png") **Local Lights Buffer Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Local Lights Buffer Renderer** component is used to render the lights for a particle system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LightType` | **[LightType](https://wiki.resonite.com/Type:LightType "Type:LightType")** | The kind of light to use. |
| `ShadowType` | **[ShadowType](https://wiki.resonite.com/Type:ShadowType "Type:ShadowType")** | The light's shadow type. |
| `ShadowStrength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The light's shadow strength. |
| `ShadowNearPlane` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The light's near plane. |
| `ShadowMapResolution` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The light's shadow map resolution. |
| `ShadowBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The light's shadow bias. |
| `ShadowNormalBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The light's normal bias. |
| `Cookie` | **[ITexture](https://wiki.resonite.com/Type:ITexture "Type:ITexture")** | The texture used for the spotlight cutout texture. |

Fields
Collapse

## Usage

Used in particle systems.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Light](https://wiki.resonite.com/Component:Light "Component:Light")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocalLightsBufferRenderer&oldid=103838](https://wiki.resonite.com/index.php?title=Component:LocalLightsBufferRenderer&oldid=103838)"

Contents