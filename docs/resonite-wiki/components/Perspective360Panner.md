# Component:Perspective360Panner

> Source: https://wiki.resonite.com/Component:Perspective360Panner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Perspective360Panner&diff=90399) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7c/Perspective360PannerComponent.png/510px-Perspective360PannerComponent.png)](https://wiki.resonite.com/File:Perspective360PannerComponent.png) **Perspective360 Panner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Perspective360Panner** component allows for moving or panning across 360 degrees around a view, given the parameters of how this panning should work. This is mostly seen in the [WorldListFacetPreset](https://wiki.resonite.com/Component:WorldListFacetPreset "Component:WorldListFacetPreset") component, where each listed item has this component to allow looking around in the [world](https://wiki.resonite.com/World "World") preview thumbnails.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IdleFOV` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field of view used when not looking around. |
| `HoverFOV` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field of view used when looking around. |
| `FOVSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field of view speed. |
| `HorizontalPanningAcceleration` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to pick up speed. |
| `HorizontalPanningSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The horizontal panning speed. |
| `VerticalPanningSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The vertical panning speed. |
| `VerticalRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The vertical range of this field of view. |
| `AngleOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field of view angle offset. |
| `FOV` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The 2D field of view. |

Fields
Collapse

## Usage

Useful as a way of looking around any 360 type of image.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Perspective360Panner&oldid=90399](https://wiki.resonite.com/index.php?title=Component:Perspective360Panner&oldid=90399)"

Contents