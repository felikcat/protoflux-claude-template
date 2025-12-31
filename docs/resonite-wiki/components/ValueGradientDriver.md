# Component:ValueGradientDriver

> Source: https://wiki.resonite.com/Component:ValueGradientDriver

Other languages:

- English
- [日本語](https://wiki.resonite.com/Component:ValueGradientDriver/ja "コンポーネント:ValueGradientDriver`1 (12% translated)")

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/60/ValueGradientDriver%601Component.png/510px-ValueGradientDriver%601Component.png)](https://wiki.resonite.com/File:ValueGradientDriver%601Component.png) **ValueGradientDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueGradientDriver** component changes the value of the field defined in `Target` based on the items in the `Points` list and their `Position` in relation to the `Progress` value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Progress` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls which items from the `Points` list will be used to drive the value of `Target` |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field that this component will drive the value of |
| `Interpolate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component will interpolate (or blend) between the nearest two `Points` to the current `Progress` value. |
| `Points` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ValueGradientDriver\`1.Point](https://wiki.resonite.com/Component:ValueGradientDriver#Point) <T>** | A list of items indicating their `Position` (in relation to `Progress`), and a `Value` |

Fields
Collapse

## Usage

Each point in the `Points` list has a `Position` field and `Value` field. The `Position` field is used for comparison with the component's `Progress` field, while the `Value` field is the value used for driving the field in `Target`.

When `Interpolate` is checked, the value stored in `Target` is linearly interpolated between the `Value`s of the two points surrounding the current `Progress`. When unchecked, the output value is simply set to the `Value` of the closest point before the current `Progress`. The only exception to this is when no point exists before the current `Progress`, in which case the first point after the current `Progress` is used.

If two points have the same `Position`, then the point of greatest index takes priority if the value is not interpolated or if the positions are exactly equal to the current `Progress`. _During_ interpolation, however, the point of _least_ index takes priority.

## Examples

- Play Video





Local File









Local File might collect personal data.



ContinueDismiss






[https://wiki.resonite.com/File:Component\_example\_ValueGradientDriver.webm](https://wiki.resonite.com/File:Component_example_ValueGradientDriver.webm)

General usage of the component, showing interpolation and non-interpolation between five float values.

- [![A ValueGradientDriver is set up with five int values. The progress is fixed at 1 and each point's value is set to its index. Interpolation is disabled. The index of the point with the greatest position is output.](https://wiki.resonite.com/images/thumb/a/a1/Component_example_ValueGradientDriver_IndexOfMax.webp/560px-Component_example_ValueGradientDriver_IndexOfMax.webp.png)](https://wiki.resonite.com/File:Component_example_ValueGradientDriver_IndexOfMax.webp "An unorthodox yet valid usage of the component, as way to find the index of the maximum value in a list of floats (as the Position values) without the need for ProtoFlux. Progress may be set to 0 to find the index of the minimum value as well.")

An unorthodox yet valid usage of the component, as way to find the index of the maximum value in a list of floats (as the `Position` values) without the need for ProtoFlux. `Progress` may be set to 0 to find the index of the minimum value as well.


Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueGradientDriver&oldid=113029](https://wiki.resonite.com/index.php?title=Component:ValueGradientDriver&oldid=113029)"

Contents