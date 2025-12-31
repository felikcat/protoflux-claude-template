# Component:VolumePlaneSlicer

> Source: https://wiki.resonite.com/Component:VolumePlaneSlicer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c5/VolumePlaneSlicerComponent.png/510px-VolumePlaneSlicerComponent.png)](https://wiki.resonite.com/File:VolumePlaneSlicerComponent.png) **Volume Plane Slicer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Volume Unlit Material Examples section](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Examples "Component:VolumeUnlitMaterial") for better information on how slicers work.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mode` | **[VolumePlaneMode](https://wiki.resonite.com/Type:VolumePlaneMode "Type:VolumePlaneMode")** | The kind of slicer mode this slicer is doing. |
| `HighlightColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color highlight to highlight the slicer with. please see [Volume Unlit Material Examples section](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Examples "Component:VolumeUnlitMaterial") for better info. |
| `HighlightRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The color highlight range to use. please see [Volume Unlit Material Examples section](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Examples "Component:VolumeUnlitMaterial") for better info. |
| `_colorDialog` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The dialog ui currently being used to choose a color to display for the color highlight. |
| `_grabGrid` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to enable when grabbing the slicer to show the grid visual. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SelectColor:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user requests to use the slicer. |

Triggers
Collapse

## Usage

See [Volume Unlit Material Examples section](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Examples "Component:VolumeUnlitMaterial").

## Examples

See [Volume Unlit Material Examples section](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Examples "Component:VolumeUnlitMaterial").

## See Also

- [Volume Unlit Material Examples section](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Examples "Component:VolumeUnlitMaterial").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VolumePlaneSlicer&oldid=100809](https://wiki.resonite.com/index.php?title=Component:VolumePlaneSlicer&oldid=100809)"

Contents