# Component:LegacyEnumEditor

> Source: https://wiki.resonite.com/Component:LegacyEnumEditor

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3c/LegacyEnumEditor%601Component.png/510px-LegacyEnumEditor%601Component.png)](https://wiki.resonite.com/File:LegacyEnumEditor%601Component.png) **Legacy Enum Editor\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyEnumEditor** component is used to cycle between enums. It is Legacy content migrated from other platforms. This should not be used, and replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the UI. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the UI |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the UI. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick the UI is. |
| `Slant` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The beveledness of the UI elements. |
| `_textSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the text visual for the enum indicator |
| `_textRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer of the enum indcator. |
| `_textEditor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | The text editor for editing the enum text. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the UI. |
| `_mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of the ui. |
| `_textBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field that is used to make the UI wrap around the text |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of the collider for the UI. |
| `_meshLeft` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of the left cycle button |
| `_meshRight` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of the right cycle button |
| `_textLeftBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to make the UI wrap around the left button text. |
| `_textRightBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to make the UI wrap around the right button text. |
| `_leftTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The renderer for the text of the left button. |
| `_rightTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The renderer for the text of the right button. |
| `_colliderLeftSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider field to drive to make the collider envelop the left UI. |
| `_colliderRightSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the collider firld to drive to make the collider envelop the right UI. |
| `_leftOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left button offset. |
| `_rightOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the right button offset. |
| `_leftTextPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the left text position. |
| `_rightTextPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the right text position. |
| `IsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `Value` | **E** | The Enum that this component has selected. |
| `_textDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string field to drive with the string version of the selected enum from `Value`. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``EditingStarted:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the enum text field is entered into. |
| ``EditingChanged:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the enum text field is changed. |
| ``EditingFinished:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the enum text field is finished with editing. |
| `OnLeftTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the left button is touched. |
| `OnRightTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the right button is touched. |

Triggers
Collapse

## Usage

When attaching, the component needs an Enum type for **E**.
But just don't use this component for new content at all.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyEnumEditor&oldid=99015](https://wiki.resonite.com/index.php?title=Component:LegacyEnumEditor&oldid=99015)"

Contents