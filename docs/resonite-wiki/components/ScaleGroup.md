# Component:ScaleGroup

> Source: https://wiki.resonite.com/Component:ScaleGroup

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScaleGroup&diff=100691) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a3/ScaleGroupComponent.png/510px-ScaleGroupComponent.png)](https://wiki.resonite.com/File:ScaleGroupComponent.png) **Scale Group** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleGroup** component is used to make a touchable selection system that can be used to select items like the Steamtm store and big picture menus.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SelectedElement` | **[ScaleElement](https://wiki.resonite.com/Component:ScaleElement "Component:ScaleElement")** | The currently selected element for this group. |
| `IdleScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of elements when they aren't selected. |
| `BackgroundScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of elements when they go into the background. |
| `SelectedScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of any element when it is selected. |
| `SmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed at which elements change scale when they change state. |

Fields
Collapse

## Usage

Used with a [Scale Element](https://wiki.resonite.com/Component:ScaleElement "Component:ScaleElement") list to make a list of selectable elements. Using ProtoFlux to get the slot of the `SelectedElement` can make this useful for a physical based selection system usable in both VR and Desktop.

## Examples

Item made by brecert that shows the component in action on 5 clickable boxes, that grow to the ScaleGroup's `SelectedScale` when clicked.
`resdb:///3bfbdceb6a3ed18ede90032c291ddd9051682f6e454ba1d3b2ba14d34e84c884.brson`

## See Also

- [Component:ScaleElement](https://wiki.resonite.com/Component:ScaleElement "Component:ScaleElement")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleGroup&oldid=100691](https://wiki.resonite.com/index.php?title=Component:ScaleGroup&oldid=100691)"

Contents