# Component:OSC Sender

> Source: https://wiki.resonite.com/Component:OSC_Sender

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d3/OSC_SenderComponent.png/510px-OSC_SenderComponent.png)](https://wiki.resonite.com/File:OSC_SenderComponent.png) **OSC Sender** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OSC\_Sender** component will try to connect to the OSC Server at the URL provided, and send data to it.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HandlingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The OSC Sender finds the OSC server on this User's machine. |
| `AccessReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Displayed in the Host Access Dialog when a connection is trying to be established. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | Uri of the OSC Server to connect to, must be in the format `osc://<ip>:<port>. E.g. osc://127.0.0.1:3001<br>` |
| `LocalPort` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Sets the local port. Defaults on 0 which is random. |
| `IsSending` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Set to true if this OSC Sender is sending data. |
| `SendMode` | **[OSC\_SendMode](https://wiki.resonite.com/Type:OSC_SendMode "Type:OSC SendMode")** | The Mode in which data is sent to the OSC Server. See [#Usage](https://wiki.resonite.com/Component:OSC_Sender#Usage) |
| `AutoResendInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Data will automatically be resent at this interval if it is set. In Seconds. See [#Behavior](https://wiki.resonite.com/Component:OSC_Sender#Behavior) |

Fields
Collapse

## Usage

Once `Handling User` and `Uri` are set, this component will try to connect to the OSC Server at the URL provided. To actually receive data, you should use the Value components:

- [Component:OSC\_Value](https://wiki.resonite.com/Component:OSC_Value "Component:OSC Value")
- [Component:OSC\_Field](https://wiki.resonite.com/Component:OSC_Field "Component:OSC Field")

## Examples

- See [OSC](https://wiki.resonite.com/OSC "OSC")

## Limits

When sending Multi-Dimensional OSC Values, there is a limit of 256 values on a single OSC Path.

There are no limits to the number of OSC Paths that can be used.

## See Also

- [Component:OSC\_Receiver](https://wiki.resonite.com/Component:OSC_Receiver "Component:OSC Receiver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OSC\_Sender&oldid=102073](https://wiki.resonite.com/index.php?title=Component:OSC_Sender&oldid=102073)"

Contents