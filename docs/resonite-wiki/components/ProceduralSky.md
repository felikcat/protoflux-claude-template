# Component:ProceduralSky

> Source: https://wiki.resonite.com/Component:ProceduralSky

Collapse **Component image**

[File:ProceduralSkyComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProceduralSkyComponent.png "File:ProceduralSkyComponent.png") **Procedural Sky** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProceduralSky** texture is used to dynamically create a skybox using a sun rotation and intensity including sun color.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SunQuality` | **[ProceduralSky.SunType](https://wiki.resonite.com/Component:ProceduralSky#SunType)** | The quality preset of the sun in the sky. |
| `SunSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | size of the sun in the sky |
| `Sun` | **[Light](https://wiki.resonite.com/Component:Light "Component:Light")** | The light to use for rotation, intensity, and color of the sun on this material. |
| `AtmosphereThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the atmosphere will light up the scene. If this is low, the `SkyTint` color coming up from the lower region of the world won't make it up to the top of the world as well, and will gradient into black. good for thin atmosphere planets, or 0 for no atmosphere. |
| `SkyTint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The tint of the atmosphere of the world. |
| `GroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The tint of the sky below the horizon line. |
| `Exposure` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to light up or darken the sky color overall. |

Fields
Collapse

## SunType

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | There should be no sun texture in the sky. |
| `Simple` | 1 | There should be a simple disk for the sun texture in the sky. |
| `HighQuality` | 2 | There should be a disk with a feathered/gradient edge for the sun texture in the sky. |

Values

## Usage

## Examples

[![](https://wiki.resonite.com/images/thumb/8/8b/ProceduralSky_Example_1.png/600px-ProceduralSky_Example_1.png)](https://wiki.resonite.com/File:ProceduralSky_Example_1.png) Example of a procedural sky using a sun size of 0.2, an atmospheric thickness of 0.2, a sun quality of high, and a sun color of cyan close to the horizon.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProceduralSky&oldid=106260](https://wiki.resonite.com/index.php?title=Component:ProceduralSky&oldid=106260)"

Contents