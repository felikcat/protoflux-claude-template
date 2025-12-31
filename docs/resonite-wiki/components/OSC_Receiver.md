# Component:OSC Receiver

> Source: https://wiki.resonite.com/Component:OSC_Receiver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/22/OSC_ReceiverComponent.png/510px-OSC_ReceiverComponent.png)](https://wiki.resonite.com/File:OSC_ReceiverComponent.png) **OSC Receiver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OSC\_Reciever** component creates an OSC Server within Resonite to receive OSC messages.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

If this component does not work as expected, try disabling and re-enabling the `Enabled` field.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HandlingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The OSC Reciever creates the OSC server on this User's machine. |
| `AccessReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Displayed in the Host Access Dialog when a connection is trying to be established. |
| `Port` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Network port to listen on for OSC connections |
| `IsListening` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This value is set to true when Resonite is successful in opening a network connection to receive data on. |

Fields
Collapse

## Usage

Once `Handling User` and `Port` are set, To actually receive data, you should use the Value components:

- [Component:OSC\_Value](https://wiki.resonite.com/Component:OSC_Value "Component:OSC Value")
- [Component:OSC\_Field](https://wiki.resonite.com/Component:OSC_Field "Component:OSC Field")

## Examples

- See [OSC](https://wiki.resonite.com/OSC "OSC").

## Limits

There are no limits to the number of OSC Paths that can be used to receive data.

When using a Headless Server the OSC address must be set to "localhost", using 127.0.0.1 will not work.

## See Also

- [OSC](https://wiki.resonite.com/OSC "OSC")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OSC\_Receiver&oldid=93768](https://wiki.resonite.com/index.php?title=Component:OSC_Receiver&oldid=93768)"

Contents