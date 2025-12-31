# Component:TouchValueOption

> Source: https://wiki.resonite.com/Component:TouchValueOption

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fb/TouchValueOption%601Component.png/510px-TouchValueOption%601Component.png)](https://wiki.resonite.com/File:TouchValueOption%601Component.png) **Touch Value Option\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchValueOption** component allows you to set a field to a value on press, it can drive indicators for Active and Hovering.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The field to set. |
| `Value` | **T** | The value to set `Target` to. |
| `ActiveIndicator` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether **T** in `Target` equals `Value`. |
| `HoverIndicator` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether this button is being hovered over via laser. |
| `HoverVibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate haptics on the hand that is hovering over this option. |
| `Vibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | How to vibrate haptics on the hand that is pressing this option. |
| `SetOnTouchBegin` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the **T** in `Target` to `Value` upon start touching this component. |
| `SetOnTouchStay` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the **T** in `Target` to `Value` every frame while keeping touching this component. |
| `SetOnTouchEnd` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the **T** in `Target` to `Value` upon end touching this component. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component can only be interacted with if the user is in edit mode. |
| `ActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether only the active user of this component can interact with this component. |

Fields
Collapse

## Usage

Needs a static collider on the same slot in order to work. Attach to said slot and provide a field for it to set in `Target`.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:TouchToggle](https://wiki.resonite.com/Component:TouchToggle "Component:TouchToggle")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchValueOption&oldid=95766](https://wiki.resonite.com/index.php?title=Component:TouchValueOption&oldid=95766)"

Contents