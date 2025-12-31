# Component:ButtonDynamicImpulseTrigger

> Source: https://wiki.resonite.com/Component:ButtonDynamicImpulseTrigger

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2a/ButtonDynamicImpulseTriggerComponent.png/510px-ButtonDynamicImpulseTriggerComponent.png)](https://wiki.resonite.com/File:ButtonDynamicImpulseTriggerComponent.png) **Button Dynamic Impulse Trigger** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonDynamicImpulseTrigger** component sends [Dynamic Impulses](https://wiki.resonite.com/Dynamic_Impulses "Dynamic Impulses") to [flux node receivers](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver "ProtoFlux:Dynamic Impulse Receiver"). This acts like a combination of [Button Events](https://wiki.resonite.com/ProtoFlux:Button_Events "ProtoFlux:Button Events") & [Dynamic Impulse Trigger](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger "ProtoFlux:Dynamic Impulse Trigger") [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") nodes, but as a component instead.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot hierarchy to send this impulse through. If this is null, it will pulse through root instead. |
| `ExcludeDisabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, this pulse will ignore disabled [slots](https://wiki.resonite.com/Slot "Slot"). |
| `PressedTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | When the button is pressed, send a pulse for receivers looking for this tag. |
| `PressingTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | When the button is pressing, send a pulse for receivers looking for this tag. |
| `ReleasedTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | When the button is released, send a pulse for receivers looking for this tag. |
| `HoverEnterTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | When the button just began to hover, send a pulse for receivers looking for this tag. |
| `HoverStayTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | When the button is hovering, send a pulse for receivers looking for this tag. |
| `HoverLeaveTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | When the button has stopped hovering, send a pulse for receivers looking for this tag. |

Fields
Collapse

## Usage

Useful for sending dynamic pulses cleanly instead of using flux.

## Examples

## See Also

- [ProtoFlux:Dynamic Impulse Trigger](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger "ProtoFlux:Dynamic Impulse Trigger")
- [ProtoFlux:Dynamic Impulse Receiver](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver "ProtoFlux:Dynamic Impulse Receiver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonDynamicImpulseTrigger&oldid=90349](https://wiki.resonite.com/index.php?title=Component:ButtonDynamicImpulseTrigger&oldid=90349)"

Contents