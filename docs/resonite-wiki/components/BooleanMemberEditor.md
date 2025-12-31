# Component:BooleanMemberEditor

> Source: https://wiki.resonite.com/Component:BooleanMemberEditor

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BooleanMemberEditor&diff=93863) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5b/BooleanMemberEditorComponent.png/510px-BooleanMemberEditorComponent.png)](https://wiki.resonite.com/File:BooleanMemberEditorComponent.png) **Boolean Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BooleanMemberEditor** component is commonly used in [Scene Inspectors](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") to allow toggling of booleans even if they are a sub property of a type like a [Bool3](https://wiki.resonite.com/Type:Bool3 "Type:Bool3") Using `_path`. This can be utilized in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether editing of this field instantly updates the `_target`. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The sub path under `_target`. This can be something like "x" to represent the first value of a [Bool3](https://wiki.resonite.com/Type:Bool3 "Type:Bool3") field. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The bool field or a field with a toggleable bool subfield. |
| `_checkBox` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The Checkbox to toggle `_target`->`_path` with. |
| `_stateDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with the state of `_target`->`_path` |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to toggle `_target`->`_path` with. |

Fields
Collapse

## Usage

Used in [Scene Inspectors](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## See Also

- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")
- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanMemberEditor&oldid=93863](https://wiki.resonite.com/index.php?title=Component:BooleanMemberEditor&oldid=93863)"

Contents