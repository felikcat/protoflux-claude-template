# Component:TextEditor

> Source: https://wiki.resonite.com/Component:TextEditor

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TextEditor&diff=97774) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c3/TextEditorComponent.png/510px-TextEditorComponent.png)](https://wiki.resonite.com/File:TextEditorComponent.png) **Text Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextEditor** component takes in a reference to a [Text](https://wiki.resonite.com/Component:Text "Component:Text") or [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer"), and then outputs the result into that reference along with the parameters given and by what actions it should do so.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Text` | **[IText](https://wiki.resonite.com/Type:IText "Type:IText")** | The output of where the text is going to be placed at. |
| `Undo` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, the setting of the text is undoable. |
| `UndoDescription` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | This gets shown on the undo button on the [Context menu](https://wiki.resonite.com/Context_menu "Context menu"). |
| `FinishHandling` | **[TextEditor.FinishAction](https://wiki.resonite.com/Component:TextEditor#FinishAction)** | Lets the Text editor know what to do when the user leaves a text input. |
| `AutoCaretColorField` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Automatically sets the color of the caret (based on text color). |
| `CaretColorField` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Sets the caret color. |
| `SelectionColorField` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Sets the selection color for this caret. |
| `EditingStarted` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <TextEditor>** | Gives the TextEditor an action when the editing has started. |
| `EditingChanged` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <TextEditor>** | Gives the TextEditor an action when the editing has changed. |
| `EditingFinished` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <TextEditor>** | Gives the TextEditor an action when the editing has finished. |
| `SubmitPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <TextEditor>** | Gives the TextEditor an action when the editing has been submitted. |

Fields
Collapse

## Usage

This component is used in many places, including:

- [Primitive Member Editor](https://wiki.resonite.com/Component:PrimitiveMemberEditor "Component:PrimitiveMemberEditor") for directly editing [TextFields](https://wiki.resonite.com/Component:TextField "Component:TextField") (and [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking"))
- [UIX](https://wiki.resonite.com/UIX "UIX") and [TextFields](https://wiki.resonite.com/Component:TextField "Component:TextField")
- [Parsing floats](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") and [parsing ints](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextEditor&oldid=97774](https://wiki.resonite.com/index.php?title=Component:TextEditor&oldid=97774)"

Contents