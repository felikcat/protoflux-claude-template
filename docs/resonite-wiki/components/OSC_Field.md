# Component:OSC Field

> Source: https://wiki.resonite.com/Component:OSC_Field

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d2/OSC_Field%601Component.png/510px-OSC_Field%601Component.png)](https://wiki.resonite.com/File:OSC_Field%601Component.png) **OSC Field\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OSC\_Field\`1** Component is used to send and recieve [OSC data](https://wiki.resonite.com/OSC "OSC").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Handler` | **[OSC\_Handler](https://wiki.resonite.com/Type:OSC_Handler "Type:OSC Handler")** | The [Component:OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver") or [Component:OSC\_Sender](https://wiki.resonite.com/Component:OSC_Sender "Component:OSC Sender") to be used with this field. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The OSC Path for this value. |
| `ArgumentIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | For [Multi-Dimensional OSC Values](https://wiki.resonite.com/OSC#Multi-Dimensional_Values "OSC"), this specifies which value to retrieve or send. |
| `Field` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The Field to store the value in. |

Fields
Collapse

## Usage

### Receiving

When `Handler`, is set to a valid and `IsListening`, [OSC Reciever](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver"), if [OSC](https://wiki.resonite.com/OSC "OSC") Data is found at the specified `Path`. The value from OSC will be set on the Field specified.

### Sending

When `Handler`, is set to a valid, [OSC Sender](https://wiki.resonite.com/Component:OSC_Sender "Component:OSC Sender").

If the `SendMode` of the [OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver"), is set to `SendAsBundles`, then it will bundle up all other OSC Value component's values and send them all as a bundle.

If the `SendMode` of the [OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver"), is set to `SendIndividually`, then Resonite will send the value within the specified `Field`, as an OSC message on the OSC Path in `Path`.

Resonite will send data each time it changes or again every `AutoResendInterval` on the [OSC\_Sender](https://wiki.resonite.com/Component:OSC_Sender "Component:OSC Sender").

## Examples

- See [OSC](https://wiki.resonite.com/OSC "OSC")

## See Also

- [OSC](https://wiki.resonite.com/OSC "OSC")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OSC\_Field&oldid=93767](https://wiki.resonite.com/index.php?title=Component:OSC_Field&oldid=93767)"

Contents