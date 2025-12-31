# Component:AuthorityTimeBase

> Source: https://wiki.resonite.com/Component:AuthorityTimeBase

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3d/AuthorityTimeBaseComponent.png/510px-AuthorityTimeBaseComponent.png)](https://wiki.resonite.com/File:AuthorityTimeBaseComponent.png) **AuthorityTimeBase** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AuthorityTimeBase** component allows for fine-grained control over the world time with a certain speed and with respect to a given offset.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BaseSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Speed of the time base. |
| `_actualSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Actual speed of the time base. Should not be written to or driven. |
| `_actualOffset` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | Offset of the time base from the current world time. Can be written to or driven perfectly fine. |

Fields
Collapse

## Usage

The output of the component is the current world time (as a [Double](https://wiki.resonite.com/Type:Double "Type:Double")) multiplied by the `BaseSpeed`, minus the `_actualOffset`.

The output of the component is accessed by [sourcing](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") the component itself. To write to the current time of the component, you write to said source. When writing to the component source, `_actualOffset` is automatically updated to reflect the correct time. When writing to `BaseSpeed`, `_actualOffset` is automatically updated to keep the same time. Writing to `_actualOffset` does not affect any other fields.

## Examples

[![](https://wiki.resonite.com/images/thumb/5/50/AuthorityTimeBase_ProtoFlux.png/500px-AuthorityTimeBase_ProtoFlux.png)](https://wiki.resonite.com/File:AuthorityTimeBase_ProtoFlux.png) An example that displays the currently computed time, allows it to be set back to 0 and that sets the speed to go forward (+1) or backward (-1) in time

## See Also

- [ProtoFlux:World Time Double](https://wiki.resonite.com/ProtoFlux:World_Time_Double "ProtoFlux:World Time Double")
- [ProtoFlux:World Time Float](https://wiki.resonite.com/ProtoFlux:World_Time_Float "ProtoFlux:World Time Float")
- [ProtoFlux:Estimated Master Clock Error](https://wiki.resonite.com/ProtoFlux:Estimated_Master_Clock_Error "ProtoFlux:Estimated Master Clock Error")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AuthorityTimeBase&oldid=93378](https://wiki.resonite.com/index.php?title=Component:AuthorityTimeBase&oldid=93378)"

Contents