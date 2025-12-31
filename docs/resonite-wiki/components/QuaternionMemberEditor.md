# Component:QuaternionMemberEditor

> Source: https://wiki.resonite.com/Component:QuaternionMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e1/QuaternionMemberEditorComponent.png/510px-QuaternionMemberEditorComponent.png)](https://wiki.resonite.com/File:QuaternionMemberEditorComponent.png) **Quaternion Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **QuaternionMemberEditor** component is a low-level component for use in editing [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") elements as XYZ Euler angles in degrees. It is used, for example, in the ProtoFlux input node for FloatQ values.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This can be used for [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking"), and isn't meant to really be used by the user due to being in uncategorized. use at your own risk.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes update a value instantly. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | see [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking"). essentially accesses a member underneath another one. for example, "x" will access the x element of a Float3, Float2, Float4, or FloatQ. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | Target field, which should be a FloatQ. |
| `Vertical` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the target UI is a vertical layout, as opposed to a horizontal layout. |
| `_xEditor` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | TextEditor for the X field. |
| `_yEditor` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | TextEditor for the Y field. |
| `_zEditor` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | TextEditor for the Z field. |
| `_xDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Field to be driven by the X angle. Should be the `Content` field on the [Text](https://wiki.resonite.com/Component:Text "Component:Text") component that `_xEditor` is pointing to. |
| `_yDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Field to be driven by the Y angle. |
| `_zDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | Field to be driven by the Z angle. |
| `_xButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button whose sync delegates are attached to the `_xEditor` |
| `_yButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button whose sync delegates are attached to the `_yEditor` |
| `_zButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Button whose sync delegates are attached to the `_zEditor` |
| `_editingValue` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Double3](https://wiki.resonite.com/Type:Double3 "Type:Double3") >** | The value that the user is currently entering at it's current editing state. updates continuously. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``EditingStarted:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the component has started editing. |
| ``EditingChanged:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the component's editing value changes. |
| ``EditingFinished:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the component finishes editing. |

Triggers
Collapse

## Usage

This component's behavior is very similar to [PrimitiveMemberEditor](https://wiki.resonite.com/Component:PrimitiveMemberEditor "Component:PrimitiveMemberEditor"), but a layer of abstraction exists between the FloatQ field in `_target` and the text field being driven for each member. This abstraction layer converts to and from Euler angles and quaterion values, which is then used for building a UI to edit quaternions as Euler angles.

## Examples

## See Also

- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:QuaternionMemberEditor&oldid=99107](https://wiki.resonite.com/index.php?title=Component:QuaternionMemberEditor&oldid=99107)"

Contents