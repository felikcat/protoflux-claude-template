# Component:ButtonStringErase

> Source: https://wiki.resonite.com/Component:ButtonStringErase

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonStringErase&diff=90363) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5a/ButtonStringEraseComponent.png/510px-ButtonStringEraseComponent.png)](https://wiki.resonite.com/File:ButtonStringEraseComponent.png) **Button String Erase** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonStringErase** component can be used to remove characters from the beginning or end of a [string](https://wiki.resonite.com/Type:String "Type:String") whenever an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetString` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The string from which characters will be removed. |
| `Count` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many characters to remove. |
| `EraseFromBeginning` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to remove characters from the beginning of the string. |

Fields
Collapse

## Usage

To function, the component simply needs to be attached to a [slot](https://wiki.resonite.com/Slot "Slot") that also has a button component attached to it. From then on, pressing that button will activate the **ButtonStringErase**, making it erase the first or last `Count` characters from its `TargetString`.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonStringErase&oldid=90363](https://wiki.resonite.com/index.php?title=Component:ButtonStringErase&oldid=90363)"

Contents