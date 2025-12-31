# Component:IntTextEditorParser

> Source: https://wiki.resonite.com/Component:IntTextEditorParser

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:IntTextEditorParser&diff=90405) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3c/IntTextEditorParserComponent.png/510px-IntTextEditorParserComponent.png)](https://wiki.resonite.com/File:IntTextEditorParserComponent.png) **Int Text Editor Parser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **IntTextEditorParser** component takes in a `ParsedValue` and if there is a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") on the same [slot](https://wiki.resonite.com/Slot "Slot"), it will send the value through the text editor and into either a [Text](https://wiki.resonite.com/Component:Text "Component:Text") or a [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer") component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParseContinuously` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, makes the value always update and parse. If false, it only updates when submitted. |
| `UpdateStringFromValue` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, will update the string value from this parsed value. |
| `ParsedValue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The value that was read from the text field. |
| `Min` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The minimum value that can be read. |
| `Max` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum value that can be read. |
| `Increments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The output value will round down to the nearest increment multiple of this value. |
| `StringFormat` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Lets you format the string for the text output. |

Fields
Collapse

## Usage

Place on the same [Slot](https://wiki.resonite.com/Slot "Slot") as a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") and anything entered into the text editor will be attempted to be parsed as a Int and output via the `ParsedValue` field.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:IntTextEditorParser&oldid=90405](https://wiki.resonite.com/index.php?title=Component:IntTextEditorParser&oldid=90405)"

Contents