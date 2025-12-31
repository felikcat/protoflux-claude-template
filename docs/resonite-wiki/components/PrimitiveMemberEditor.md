# Component:PrimitiveMemberEditor

> Source: https://wiki.resonite.com/Component:PrimitiveMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c6/PrimitiveMemberEditorComponent.png/510px-PrimitiveMemberEditorComponent.png)](https://wiki.resonite.com/File:PrimitiveMemberEditorComponent.png) **Primitive Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PrimitiveMemberEditor** component is a lower-level component for accessing and editing the members of a particular primitive element. Its intention is for use in [Scene Inspectors](https://wiki.resonite.com/Scene_Inspector_Dialog "Scene Inspector Dialog"), since they use a text field to drive member properties, but it can be more generally used on player-made objects as well. It is also, as indicated by a big warning on it, commonly used for [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking") due to being able to read and write the `id` field of a [RefID](https://wiki.resonite.com/Type:RefID "Type:RefID").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to update the target field while editing the text field. If disabled, it will only update at the end of editing. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Member path of target element field to access/edit. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The primitive element to access/edit. |
| `Format` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The format for representing the target primitive. About the same as the Format field for the [To String](https://wiki.resonite.com/ProtoFlux:To_String "ProtoFlux:To String") node, but only works on a limited set of primitives. |
| `_textEditor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | The TextEditor that points to any component that implements the [IText type](https://wiki.resonite.com/Type:IText "Type:IText") used for `_textDrive`. |
| `_textDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Text field used as an interface to the member. Should be the `Content` field of a component implementing [IText](https://wiki.resonite.com/Type:IText "Type:IText"). |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button used for editing, like on a [TextField](https://wiki.resonite.com/Component:TextField "Component:TextField"). |
| `_resetButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button used to reset the value. Intended to only be used for strings. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``EditingStarted:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when starting editing using this component. |
| ``EditingChanged:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when changing the value during editing using this component. |
| ``EditingFinished:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when finishing editing using this component. |
| `OnReset:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when resetting the value of this component's target. |

Triggers
Collapse

## Usage

This component needs, at minimum, `_target` to point to an element with fields, a `_textDrive` that points to the `Content` field of a component implementing [IText](https://wiki.resonite.com/Type:IText "Type:IText"), and a `_textEditor` that points to a TextEditor with its `Text` field pointing to the to the aforementioned IText component. The `_textDrive` field acts as a drive with write back, allowing one to interface with the field it points to, by way of a [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") node or the `_textEditor`, to change the `_target` via the text field.

Additionally, there exists three [Sync Delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") one may apply to the `_textEditor`. These sync delegates are not strictly required for functionality of the component, but they do make the editing experience nicer if one hooks some editable field up to the TextEditor. `EditingStarted` breaks the `_textDrive` drive when called, allowing for more flexible editing by not requiring the text always be a parsable number. `EditingChanged` is only functional when `Continuous` is used, and it writes the current text to the `_target` every time the text is changed, hence being continuous. `EditingFinished` restores the `_textDrive` to before and writes the text value into `_target`, and is required for proper functionality of this component if `EditingStarted` is also used. The final sync delegate of the component, `OnReset`, is not needed unless one wishes to add a reset button. When it is called, it will simply reset the `_target` value to the type's default value.

One may fill in the `_button` and `_resetButton` fields. These fields are not too terribly useful, as they don't provide much functionality themselves (rather the Sync Delegates do), but they are used when internally building the Inspector UI and when _any part_ of the component is changed. When any part of the component changes, including when the field it is pointing to is edited, if `_button` is filled, all colors in the `ColorDrivers` list will be set to the first color drive. If `_resetButton` is filled, its slot will disable if the field that the component is editing is not a [string](https://wiki.resonite.com/Type:String "Type:String"), which can be worked around by driving the `Enabled` state of the slot to `true`.

## Examples

Due to the nature of this component, it is difficult to provide examples in images. However, there does exist in-game examples to look at.

- `resrec:///U-yosh/R-8bf5c7c2-355e-4385-bb15-fdc24043ef72`

## See Also

- [Component:BooleanMemberEditor](https://wiki.resonite.com/Component:BooleanMemberEditor "Component:BooleanMemberEditor")
- [Component:ColorMemberEditor](https://wiki.resonite.com/Component:ColorMemberEditor "Component:ColorMemberEditor")
- [Component:ColorXMemberEditor](https://wiki.resonite.com/Component:ColorXMemberEditor "Component:ColorXMemberEditor")
- [Component:EnumMemberEditor](https://wiki.resonite.com/Component:EnumMemberEditor "Component:EnumMemberEditor")
- [Component:NullableMemberEditor](https://wiki.resonite.com/Component:NullableMemberEditor "Component:NullableMemberEditor")
- [Component:QuaternionMemberEditor](https://wiki.resonite.com/Component:QuaternionMemberEditor "Component:QuaternionMemberEditor")
- [Component:SliderMemberEditor](https://wiki.resonite.com/Component:SliderMemberEditor "Component:SliderMemberEditor")
- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PrimitiveMemberEditor&oldid=99092](https://wiki.resonite.com/index.php?title=Component:PrimitiveMemberEditor&oldid=99092)"

Contents