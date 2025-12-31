# Component:FieldEditor

> Source: https://wiki.resonite.com/Component:FieldEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/36/FieldEditorComponent.png/510px-FieldEditorComponent.png)](https://wiki.resonite.com/File:FieldEditorComponent.png) **Field Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A **FieldEditor** component takes an IField of any type and deconstructs it's elements into a list of editor components.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetField` | **[IField](https://wiki.resonite.com/Type:IField "Type:IField")** | The field to generate an editor list for. |
| `_textEditors` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | A list of text editors of the specified `_targetField`'s components. |
| `_textDrives` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of text value fields to drive with the contents of the components of the specified `_targetField`. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``EditingStarted:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when editing starts, used with a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor"). |
| ``EditingChanged:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when editing value changes, used with a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor"). |
| ``EditingFinished:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when editing finishes, used with a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor"). |

Triggers
Collapse

## Usage

Attach to a slot under a [UIX Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") hiearchy with a [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") and then insert an [IField](https://wiki.resonite.com/Type:IField "Type:IField") into `_targetField` to be edited for this component to generate an editor for the elements of the specified `_targetField`.

## Examples

An [IField](https://wiki.resonite.com/Type:IField "Type:IField") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") \> will make the field editor create a list with the X y and z components of the float3 field.

## See Also

- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FieldEditor&oldid=98402](https://wiki.resonite.com/index.php?title=Component:FieldEditor&oldid=98402)"

Contents