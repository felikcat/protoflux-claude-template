# Component:LegacyTextField

> Source: https://wiki.resonite.com/Component:LegacyTextField

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/59/LegacyTextFieldComponent.png/510px-LegacyTextFieldComponent.png)](https://wiki.resonite.com/File:LegacyTextFieldComponent.png) **Legacy Text Field** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyTextField** component was used to edit text in old content migrated from other platforms. This component should not be used in new content, and should be replaced whenever possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the UI elements. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the UI. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the UI. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the UI. |
| `Slant` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How beveled the UI elements should be. |
| `_textSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the text visual of this UI element. |
| `_textRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer of this UI element. |
| `_textEditor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | The text editor that allows direct editing of the value this UI element controls. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of this UI. |
| `_mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of this UI. |
| `_textBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive with the bounds of the text to keep the UI around it. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with what the size of this UI's collider should be. |
| `_meshLeft` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of the left button. |
| `_meshRight` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of the right button. |
| `_textLeftBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive with the bounds of the text on the left button so the UI stays wrapped around it. |
| `_textRightBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive with the bounds of the text on the right button so the UI stays wrapped around it. |
| `_leftTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer of the left button. |
| `_rightTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer of the right button. |
| `_colliderLeftSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with what the size of the left collider should be. |
| `_colliderRightSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with what the size of the right collider should be. |
| `_leftOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with what the offset of the left collider should be. |
| `_rightOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with what the offset of the right collider should be. |
| `_leftTextPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive wiyh what the position of the text on the left button should be. |
| `_rightTextPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive wiyh what the position of the text on the right button should be. |
| `IsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `_hintTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | the text renderer of the edit text hint |
| `_hintTextBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the field to drive with the bounds of the hint text for keeping a UI wrapped around it. |
| `_hintTextEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the hint text should be enabled or not. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnLeftTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the left button is touched. |
| `OnRightTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the right button is touched. |

Triggers
Collapse

## Usage

Just dont.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyTextField&oldid=99060](https://wiki.resonite.com/index.php?title=Component:LegacyTextField&oldid=99060)"

Contents