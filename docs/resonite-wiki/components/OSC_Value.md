# Component:OSC Value

> Source: https://wiki.resonite.com/Component:OSC_Value

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fa/OSC_Value%601Component.png/510px-OSC_Value%601Component.png)](https://wiki.resonite.com/File:OSC_Value%601Component.png) **OSC Value\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OSC\_Value\`1** Component is used to send and recieve [OSC data](https://wiki.resonite.com/OSC "OSC").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Handler` | **[OSC\_Handler](https://wiki.resonite.com/Type:OSC_Handler "Type:OSC Handler")** | The [Component:OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver") or [Component:OSC\_Sender](https://wiki.resonite.com/Component:OSC_Sender "Component:OSC Sender") to be used with this component. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The OSC Path for this value. |
| `ArgumentIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | For [Multi-Dimensional OSC Values](https://wiki.resonite.com/OSC#Multi-Dimensional_Values "OSC"), this specifies which value to retrieve or send. |
| `Value` | **T** | The recieved OSC Value or the default value of the Type if there is no OSC data. |

Fields
Collapse

## Usage

### Receiving

When `Handler`, is set to a valid and `IsListening`, [OSC Reciever](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver"), if [OSC](https://wiki.resonite.com/OSC "OSC") Data is found at the specified `Path`. The value from OSC will be shown in the `Value` field.

### Sending

When `Handler`, is set to a valid, [OSC Sender](https://wiki.resonite.com/Component:OSC_Sender "Component:OSC Sender").

If the `SendMode` of the [OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver"), is set to `SendAsBundles`, then it will bundle up all other OSC Value component's values and send them all as a bundle.

If the `SendMode` of the [OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver"), is set to `SendIndividually`, then Resonite will send `Value`, as an OSC message on the OSC Path in `Path`.

Resonite will send data each time it changes or again every `AutoResendInterval` on the [OSC\_Sender](https://wiki.resonite.com/Component:OSC_Sender "Component:OSC Sender").

## Examples

- See [OSC](https://wiki.resonite.com/OSC "OSC")

## See Also

- [OSC](https://wiki.resonite.com/OSC "OSC")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OSC\_Value&oldid=93771](https://wiki.resonite.com/index.php?title=Component:OSC_Value&oldid=93771)"

Contents