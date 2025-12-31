# Component:WorldLoadProgress

> Source: https://wiki.resonite.com/Component:WorldLoadProgress

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/57/WorldLoadProgressComponent.png/510px-WorldLoadProgressComponent.png)](https://wiki.resonite.com/File:WorldLoadProgressComponent.png) **World Load Progress** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldLoadProgress** component is the component that controls the [WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface") behavior.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_visual` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot for the progress indicator and visual. |
| `ProgressIndicator` | **[WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")** | The loading indicator for this component. |

Fields
Collapse

## Usage

Not used by the user.

## Examples

Used in handling world load progress for load indicators.

## See Also

- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldLoadProgress&oldid=100829](https://wiki.resonite.com/index.php?title=Component:WorldLoadProgress&oldid=100829)"

Contents