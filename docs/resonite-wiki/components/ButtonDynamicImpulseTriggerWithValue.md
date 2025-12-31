# Component:ButtonDynamicImpulseTriggerWithValue

> Source: https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e6/ButtonDynamicImpulseTriggerWithValue%601Component.png/510px-ButtonDynamicImpulseTriggerWithValue%601Component.png)](https://wiki.resonite.com/File:ButtonDynamicImpulseTriggerWithValue%601Component.png) **Button Dynamic Impulse Trigger With Value\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonDynamicImpulseTriggerWithValue** component sends [Dynamic Impulses](https://wiki.resonite.com/Dynamic_Impulses "Dynamic Impulses") to [flux node receivers with data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver_With_Data "ProtoFlux:Dynamic Impulse Receiver With Data"). This acts like a combination of [Button Events](https://wiki.resonite.com/ProtoFlux:Button_Events "ProtoFlux:Button Events") & [Dynamic Impulse Trigger With Data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger_With_Data "ProtoFlux:Dynamic Impulse Trigger With Data") [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") nodes, but as a component instead.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to target with impulses specified by `PressedData`,`PressingData`,`ReleasedData`,`HoverEnterData`,`HoverStayData`,`HoverLeaveData`. |
| `ExcludeDisabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether disabled slots and hierarchies should be affected by the dynamic impulses sent. |
| `PressedData` | _direct_ **[ButtonDynamicImpulseTriggerWithValue\`1.EventData](https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue#EventData) <T>** | What value and tag type dynamic impulse to send when an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed on the same slot. |
| `PressingData` | _direct_ **[ButtonDynamicImpulseTriggerWithValue\`1.EventData](https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue#EventData) <T>** | What value and tag type dynamic impulse to send when an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is being pressed on the same slot. Fires every update while the button is being pressed. |
| `ReleasedData` | _direct_ **[ButtonDynamicImpulseTriggerWithValue\`1.EventData](https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue#EventData) <T>** | What value and tag type dynamic impulse to send when an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") stops being pressed on the same slot. |
| `HoverEnterData` | _direct_ **[ButtonDynamicImpulseTriggerWithValue\`1.EventData](https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue#EventData) <T>** | What value and tag type dynamic impulse to send when an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") starts being pointed at on the same slot. |
| `HoverStayData` | _direct_ **[ButtonDynamicImpulseTriggerWithValue\`1.EventData](https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue#EventData) <T>** | What value and tag type dynamic impulse to send when an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is currently pointed at on the same slot. Fires every update while the button is being hovered over. |
| `HoverLeaveData` | _direct_ **[ButtonDynamicImpulseTriggerWithValue\`1.EventData](https://wiki.resonite.com/Component:ButtonDynamicImpulseTriggerWithValue#EventData) <T>** | What value and tag type dynamic impulse to send when an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") stops being pointed at on the same slot. |

Fields
Collapse

## EventData

| Name | Type | Description |
| --- | --- | --- |
| `Tag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Tag of the sent impulse |
| `Value` | **T** | The value to send with the [Dynamic Impulse](https://wiki.resonite.com/Dynamic_Impulses "Dynamic Impulses") |

Fields

## Usage

Useful for sending dynamic pulses cleanly instead of using flux.

## Examples

This is useful for making a keyboard by putting this component on each button and then sending the char of the button that pressed it, so all your code can be in one place.

## See Also

- [ProtoFlux:Dynamic Impulse Trigger With Data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger_With_Data "ProtoFlux:Dynamic Impulse Trigger With Data")
- [ProtoFlux:Dynamic Impulse Receiver With Data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver_With_Data "ProtoFlux:Dynamic Impulse Receiver With Data")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonDynamicImpulseTriggerWithValue&oldid=97424](https://wiki.resonite.com/index.php?title=Component:ButtonDynamicImpulseTriggerWithValue&oldid=97424)"

Contents