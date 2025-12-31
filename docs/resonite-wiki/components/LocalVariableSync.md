# Component:LocalVariableSync

> Source: https://wiki.resonite.com/Component:LocalVariableSync

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:LocalVariableSync\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LocalVariableSync%601Component.png "File:LocalVariableSync`1Component.png") **Local Variable Sync\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocalVariableSync** component is used to store a value to the local dB for the user space and load it up again.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OwnerUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that this variable is associated with in the world. |
| `Value` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value to Sync with the local DB variable. |
| `Variable` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the local DB variable. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocalVariableSync&oldid=104699](https://wiki.resonite.com/index.php?title=Component:LocalVariableSync&oldid=104699)"

Contents