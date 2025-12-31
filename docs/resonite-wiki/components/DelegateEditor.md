# Component:DelegateEditor

> Source: https://wiki.resonite.com/Component:DelegateEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/DelegateEditorComponent.png/510px-DelegateEditorComponent.png)](https://wiki.resonite.com/File:DelegateEditorComponent.png) **Delegate Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DelegateEditor** component is used in the Inspector window of Components where there is a field a [sync delegate](https://wiki.resonite.com/Sync_Delegates "Sync Delegates") can be dropped into.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetDelegate` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ISyncDelegate](https://wiki.resonite.com/index.php?title=Type:ISyncDelegate&action=edit&redlink=1 "Type:ISyncDelegate (page does not exist)") >** | The Sync delegate to show. |
| `_textDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text field to drive with the name of the Sync delegate method. |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to interface with the Sync delegate. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `RemovePressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Remove the delegate from the delegate holding field. |
| `OpenInspectorButton:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Opens the inspector to the delegate location in the world if possible. |

Triggers
Collapse

## Usage

This isn't usually used by the user, and falls into the category of Components used in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking").

## Examples

Used in the Inspector window of a [Component:CharacterTeleporter](https://wiki.resonite.com/Component:CharacterTeleporter "Component:CharacterTeleporter") for example.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DelegateEditor&oldid=98419](https://wiki.resonite.com/index.php?title=Component:DelegateEditor&oldid=98419)"

Contents