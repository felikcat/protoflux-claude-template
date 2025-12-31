# Component:TextField

> Source: https://wiki.resonite.com/Component:TextField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TextField&diff=97775) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e6/TextFieldComponent.png/510px-TextFieldComponent.png)](https://wiki.resonite.com/File:TextFieldComponent.png) **TextField** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextField** component is used in conjunction with a [TextEditor](https://wiki.resonite.com/TextEditor_(Component) "TextEditor (Component)"), [Text](https://wiki.resonite.com/Text_(Component) "Text (Component)"), and [Button](https://wiki.resonite.com/Button_(Component) "Button (Component)") component to provide an editable text field. The Text component stores the text, the TextEditor is the editor for the text, and the Button allows the text editor to appear when then text field is selected.

You must drag a reference to the Text component into the Text property of the TextEditor in order for the editor to know what text it is editing.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Editor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | A reference to the text editor component. |
| `__text` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | Internal - The text for this field. |
| `EditingStarted` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | The editing started action. |
| `EditingChanged` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | The editing changed action. |
| `EditingFinished` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | The editing finished action. |

Fields
Collapse

## Usage

This component is useful for forms, user input, and other text based projects.

## Examples

### Videos

[ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime") made a tutorial video on TextFields:

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [Component:TouchableTextField](https://wiki.resonite.com/Component:TouchableTextField "Component:TouchableTextField")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextField&oldid=97775](https://wiki.resonite.com/index.php?title=Component:TextField&oldid=97775)"

Contents