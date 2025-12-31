# Component:GlueVisualizer

> Source: https://wiki.resonite.com/Component:GlueVisualizer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/90/GlueVisualizerComponent.png/510px-GlueVisualizerComponent.png)](https://wiki.resonite.com/File:GlueVisualizerComponent.png) **Glue Visualizer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GlueVisualizer** component is used by the [Glue Tool](https://wiki.resonite.com/Glue_Tool "Glue Tool") to visualize glue objects that are to potentially gluing objects together.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[FresnelMaterial](https://wiki.resonite.com/Component:FresnelMaterial "Component:FresnelMaterial")** | The material being used to visualize the area of effect of `Glue`. |
| `Glue` | **[Glue](https://wiki.resonite.com/Component:Glue "Component:Glue")** | The Glue component to visualize. |
| `Scale` | _direct_ **[FieldHook\`1](https://wiki.resonite.com/index.php?title=Type:FieldHook%601&action=edit&redlink=1 "Type:FieldHook`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The scale field of the visual so it wobbles. |
| `BaseScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The default or base scale of the visual. |

Fields
Collapse

## Usage

See [Glue Tool](https://wiki.resonite.com/Glue_Tool "Glue Tool").

## Examples

See [Glue Tool](https://wiki.resonite.com/Glue_Tool "Glue Tool").

## See Also

- [Glue Tool](https://wiki.resonite.com/Glue_Tool "Glue Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GlueVisualizer&oldid=98761](https://wiki.resonite.com/index.php?title=Component:GlueVisualizer&oldid=98761)"

Contents