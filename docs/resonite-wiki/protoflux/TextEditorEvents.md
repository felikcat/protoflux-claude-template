# ProtoFlux:TextEditorEvents

> Source: https://wiki.resonite.com/ProtoFlux:TextEditorEvents

Text Editor Events

EditingStarted

EditingChanged

EditingFinished

SubmitPressed

Editor

null

∅

UI

The `Text Editor Events` node takes in a global [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") reference and will listen for events from that global reference. This node fires events that relate to the TextEditor, and can be useful when you want certain things to happen when things get edited or submitted by the [user](https://wiki.resonite.com/User "User").

## Outputs

### EditingStarted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the editing has started (After the editor is focused).

### EditingChanged ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after every change during the editing.

### EditingFinished ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the editing finishes (before the editor loses focus).

### SubmitPressed ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires When the user submits the changes for the editor (called before `EditingFinished` gets fired).

## Globals

### Editor ( [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor"))

The [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") to listen from.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TextEditorEvents&oldid=110795](https://wiki.resonite.com/index.php?title=ProtoFlux:TextEditorEvents&oldid=110795)"

Contents