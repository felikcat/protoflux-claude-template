# Component:ProceduralSkyMaterial

> Source: https://wiki.resonite.com/Component:ProceduralSkyMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ProceduralSkyMaterial&diff=105868) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/22/ProceduralSkyMaterialComponent.png/510px-ProceduralSkyMaterialComponent.png)](https://wiki.resonite.com/File:ProceduralSkyMaterialComponent.png) **Procedural Sky Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Procedural Sky Material** component is used to make a on-the-fly generated skybox using a light object and some values for atmosphere and sun size.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `SunQuality` | **[SunType](https://wiki.resonite.com/Component:ProceduralSkyMaterial#SunType)** | The quality of the sun visual in the sky if any. |
| `SunSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sun in the sky. |
| `Sun` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [Light](https://wiki.resonite.com/Component:Light "Component:Light") >** | The light being used for the sun position and color. |
| `AtmosphereThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the atmosphere, which determines how high up the "blue" refraction effect seen in atmospheres. if this value is low, the blue of the sky becomes a thin band on the horizon that is faint. this would give the illusion of a thin atmosphere. |
| `SkyTint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the atmosphere in the sky. for earth this is blue. |
| `GroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the sky below the horizon. |
| `Exposure` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much exposure or brightness should be given to the sky. |

Fields
Collapse

## Usage

Used commonly in sky boxes found in grid spaces, and serves as a quick and simple way of making a sky that can be changed on the fly.

## SunType

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | No sun visible in the sky. |
| `Simple` | 1 | A simple sun visible in the sky. |
| `HighQuality` | 2 | A high quality sun visible in the sky. |

Values

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProceduralSkyMaterial&oldid=105868](https://wiki.resonite.com/index.php?title=Component:ProceduralSkyMaterial&oldid=105868)"

Contents