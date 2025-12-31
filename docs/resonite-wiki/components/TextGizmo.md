# Component:TextGizmo

> Source: https://wiki.resonite.com/Component:TextGizmo

Collapse **Component image**

[File:TextGizmoComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=TextGizmoComponent.png "File:TextGizmoComponent.png") **Text Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextGizmo** component is commonly found on newly spawned text elements and is used to quickly edit the text of a spawned text element. This component and it's visuals delete themselves after the user selects the text element using a development tip or inspector.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer") >** | The text renderer to edit the text of. |
| `_editor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | The text editor Component that targets `_target` for its editing. |
| `_editIconPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the start editing icon. |
| `_editIconScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the start editing icon. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `EditTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Is called when the user wants to start editing `_target` via using this gizmo. |

Triggers
Collapse

## Usage

## Examples

Is commonly found on Basic and Outline text elements created through the create new menu brought up via the dev tip.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextGizmo&oldid=100740](https://wiki.resonite.com/index.php?title=Component:TextGizmo&oldid=100740)"

Contents