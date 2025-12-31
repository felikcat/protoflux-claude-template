# Component:ButtonStringAppend

> Source: https://wiki.resonite.com/Component:ButtonStringAppend

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonStringAppend&diff=90362) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6c/ButtonStringAppendComponent.png/510px-ButtonStringAppendComponent.png)](https://wiki.resonite.com/File:ButtonStringAppendComponent.png) **Button String Append** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonStringAppend** component can be used to add a [string](https://wiki.resonite.com/Type:String "Type:String") to the beginning or end of a string whenever an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetString` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The string to which `AppendString` will be added. |
| `AppendString` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to add to `TargetString`. |
| `AppendInFront` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to add `AppendString` to the beginning of the string. (This does not reverse `AppendString`.) |

Fields
Collapse

## Usage

To function, the component simply needs to be attached to a [slot](https://wiki.resonite.com/Slot "Slot") that also has a button component attached to it. From then on, pressing that button will activate the **ButtonStringAppend**, making it append its `AppendString` to its `TargetString`.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonStringAppend&oldid=90362](https://wiki.resonite.com/index.php?title=Component:ButtonStringAppend&oldid=90362)"

Contents