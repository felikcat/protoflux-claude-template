# Component:ColorSky

> Source: https://wiki.resonite.com/Component:ColorSky

Collapse **Component image**

[File:ColorSkyComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ColorSkyComponent.png "File:ColorSkyComponent.png") **Color Sky** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The ColorSky component creates a skybox with a color. Currently when this component is added to a slot, it will be immediately replaced with a Skybox and a material component automatically. It exists as a stub to maintain compatibility with legacy content.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

The ColorSky component is deprecated. Use [Skybox](https://wiki.resonite.com/Component:Skybox "Component:Skybox") with a material instead.


## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Internal |
| `_gradients` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ColorSky.Gradient](https://wiki.resonite.com/Component:ColorSky#Gradient)** | Internal |

Fields
Collapse

## Behavior

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorSky&oldid=97445](https://wiki.resonite.com/index.php?title=Component:ColorSky&oldid=97445)"

Contents