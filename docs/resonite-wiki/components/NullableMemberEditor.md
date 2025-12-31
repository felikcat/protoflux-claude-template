# Component:NullableMemberEditor

> Source: https://wiki.resonite.com/Component:NullableMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/77/NullableMemberEditorComponent.png/510px-NullableMemberEditorComponent.png)](https://wiki.resonite.com/File:NullableMemberEditorComponent.png) **Nullable Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Nullable Member Editor** component is commonly used in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking") and is used to modify nullable values.

Please look into Flux or component alternatives other than this component to edit nullables.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes should instantly update a target value. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The sub element to edit via C# reflection. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The value to be modifying. |
| `NullableBaseType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type of the value stored within the nullable (for "Nullable<Float>" aka "Float?" This is "Float") |
| `_checkBox` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether the nullable has a value. |
| `_stateDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether or not the nullable has a value. |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for editing the nullable. |

Fields
Collapse

## Usage

Used in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking"). Don't use for your creations or they will break at any time.

## Examples

## See Also

- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NullableMemberEditor&oldid=105346](https://wiki.resonite.com/index.php?title=Component:NullableMemberEditor&oldid=105346)"

Contents