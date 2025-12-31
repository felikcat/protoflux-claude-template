# Component:SliderMemberEditor

> Source: https://wiki.resonite.com/Component:SliderMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1f/SliderMemberEditorComponent.png/510px-SliderMemberEditorComponent.png)](https://wiki.resonite.com/File:SliderMemberEditorComponent.png) **Slider Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SliderMemberEditor** is commonly used in inspectors and can be used for [Ref hacking](https://wiki.resonite.com/Ref_hacking "Ref hacking").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether slider values should be constantly changed every frame update. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The value underneath the target element to change. path elements are separated by ".". |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The target field to change. |
| `_slider` | **[Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The slider to trigger change events this component should use to influence `_target` |
| `_sliderValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to be used for changing `_target` |
| `_textEditor` | **[PrimitiveMemberEditor](https://wiki.resonite.com/Component:PrimitiveMemberEditor "Component:PrimitiveMemberEditor")** | The text editor to change `_target` as a number text field. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Component:Slider](https://wiki.resonite.com/Component:Slider "Component:Slider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SliderMemberEditor&oldid=106563](https://wiki.resonite.com/index.php?title=Component:SliderMemberEditor&oldid=106563)"

Contents