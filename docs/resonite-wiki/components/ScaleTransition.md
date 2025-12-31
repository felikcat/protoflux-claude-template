# Component:ScaleTransition

> Source: https://wiki.resonite.com/Component:ScaleTransition

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9d/ScaleTransitionComponent.png/510px-ScaleTransitionComponent.png)](https://wiki.resonite.com/File:ScaleTransitionComponent.png) **Scale Transition** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleTransition** component makes a slot scale from one scale state to another, disabling when fully reaching its disabled scale point. The component's scale transition state is controlled via `ShowField`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ShowField` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to be transitioning to hidden (false) or shown (true) |
| `TransitionTimeField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the transition to shown or hidden should take. |
| `ShowScaleField` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | What scale the object should transition to from `HiddenScaleField` when `ShowField` is true. |
| `HiddenScaleField` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | What scale the object should transition to from `ShowScaleField` when `ShowField` is false. |
| `CurveField` | **[CurvePreset](https://wiki.resonite.com/Type:CurvePreset "Type:CurvePreset")** | How the object should transition scale over time. |
| `_scaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to make this slot scale up and down. Usually the slot's scale field. |
| `_enabledDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive to false when the object is done scaling to hidden and drive to true when transitioning away from hidden. |

Fields
Collapse

## Usage

Attach to a slot and provide values to the proper fields. When `ShowField` is toggled, the scale and enabled fields of the component will do a little animation.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Tween](https://wiki.resonite.com/Component:Tween "Component:Tween")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleTransition&oldid=95645](https://wiki.resonite.com/index.php?title=Component:ScaleTransition&oldid=95645)"

Contents