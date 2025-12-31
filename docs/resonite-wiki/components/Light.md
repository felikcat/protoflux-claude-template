# Component:Light

> Source: https://wiki.resonite.com/Component:Light

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/LightComponent.png/510px-LightComponent.png)](https://wiki.resonite.com/File:LightComponent.png) **Light** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Light** component is used to illuminate the render scene beyond skybox illumination. This component can be used for suns, spots, and points, but not area lights.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LightType` | **[LightType](https://wiki.resonite.com/Type:LightType "Type:LightType")** | The type of light. Can be Point, Directional, or Spot. |
| `Intensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How intense the light is. This is a multiplier. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the light this source should project. |
| `ShadowType` | **[ShadowType](https://wiki.resonite.com/Type:ShadowType "Type:ShadowType")** | The type of shadow this light should use. Can be None, Hard, or Soft. |
| `ShadowStrength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How dark the shadows are. |
| `ShadowNearPlane` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far away shadows will render for this point light. |
| `ShadowMapResolution` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How detailed the resolution for shadows is in pixels. |
| `ShadowBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | added to the distance in the shadow map to ensure that pixels on the borderline definitely pass the comparison as they should. |
| `ShadowNormalBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Makes surrounding lit areas encroach upon the center shadow, making the encroached area lit too. |
| `Range` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far for the light to shine in meters, where the range represents the point where the falloff stops. |
| `SpotAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle from 0-180 when on spot light mode to project the light at. 0 is no light, 60 is like car headlights, and 180 is extreme and unrealistic. |
| `Cookie` | **[ITexture](https://wiki.resonite.com/Type:ITexture "Type:ITexture")** | The cookie texture is used to limit the light area of a spot light from a circle to a custom shape. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

[![](https://wiki.resonite.com/images/thumb/4/4b/LightCookieExample.png/300px-LightCookieExample.png)](https://wiki.resonite.com/File:LightCookieExample.png) Example showing a Cookie set on a Light with a StaticTexture2D

## See also

- [Component:Skybox](https://wiki.resonite.com/Component:Skybox "Component:Skybox")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Light&oldid=108402](https://wiki.resonite.com/index.php?title=Component:Light&oldid=108402)"

Contents