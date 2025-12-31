# Component:LegacyNumericUpDown

> Source: https://wiki.resonite.com/Component:LegacyNumericUpDown

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/43/LegacyNumericUpDownComponent.png/510px-LegacyNumericUpDownComponent.png)](https://wiki.resonite.com/File:LegacyNumericUpDownComponent.png) **Legacy Numeric Up Down** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyNumericUpDown** component comes from Legacy migrated content. This component should not be used in new content, and should be removed when possible.

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
| `_textSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot of the text for the number this component is editing. |
| `_textRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer for the number this component is editing. |
| `_textEditor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | The text editor that allows for direct editing of the number this component is editing. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material this UI is using. |
| `_mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh this UI is using. |
| `_textBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive to make the UI fit around the text. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the collider size for this UI. |
| `_meshLeft` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh being used by this component's left button. |
| `_meshRight` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh being used by this component's right button. |
| `_textLeftBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive to make the left button stay wrapped around its text. |
| `_textRightBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive to make the right button stay wrapped around its text. |
| `_leftTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer for the left button. |
| `_rightTextRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer for the right button. |
| `_colliderLeftSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider size field of the left button. |
| `_colliderRightSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider size field of the right button. |
| `_leftOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider offset field of the left button. |
| `_rightOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider offset field of the right button. |
| `_leftTextPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The text position field of the left button. |
| `_rightTextPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The text position field of the right button. |
| `DriveField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field this component should drive with `Value` |
| `AllowWriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to the value of the field targeted by `DriveField` should be written to this component's `Value` field instead. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value that this component currently has for the edited field. |
| `DecimalPoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many decimal places this component should keep track of. |
| `MinValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum possible value for `Value`. |
| `MaxValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum possible value for `Value`. |
| `IncrementValue` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to increment or decrement `Value` by when pressing the left and right buttons. |
| `IsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `_textDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string field to drive with the current `Value` for the visuals. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``EditingStarted:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the number field is focused into. |
| ``EditingChanged:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the number field is changed. |
| ``EditingFinished:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Called when the number field has stopped being edited. |
| `OnLeftTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the left button is touched. |
| `OnRightTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the right button is touched. |

Triggers
Collapse

## Usage

Just dont.

## Examples

Found in legacy content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyNumericUpDown&oldid=99023](https://wiki.resonite.com/index.php?title=Component:LegacyNumericUpDown&oldid=99023)"

Contents