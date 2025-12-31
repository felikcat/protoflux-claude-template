# Component:LegacySlider

> Source: https://wiki.resonite.com/Component:LegacySlider

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cd/LegacySliderComponent.png/510px-LegacySliderComponent.png)](https://wiki.resonite.com/File:LegacySliderComponent.png) **Legacy Slider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacySlider** component was used in old legacy content to act as a UI for adjusting a float via a slider. This component should not be used in new content and should be replaced whenever possible.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `IsEnabledField` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `IncrementPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <LegacySlider>** | The Sync delegate to call when the increment button is pressed, passing this component as an argument. |
| `DecrementPressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <LegacySlider>** | The Sync delegate to call when the decrement button is pressed, passing this component as an argument. |
| `DriveField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The float field to drive with `Value` |
| `AllowWriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes to the value of the field targeted by `DriveField` should be written back to `Value`. |
| `CreateUndoStep` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether using this UI creates an [Undo](https://wiki.resonite.com/Undo "Undo") step. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value this component is influencing. |
| `Min` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value for `Value`. |
| `Max` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value for `Value`. |
| `Increment` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to shift `Value` by when using the slider side buttons. |
| `IntegerOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Value` can only be a whole number. |
| `ColorField` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this UI. |
| `SymmetricalField` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether this UI should be symmetrical. |
| `WidthField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of this UI. |
| `HeightField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of this UI. |
| `CursorRatioField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the size of the slider cursor compared to the slider container. |
| `ThicknessField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the thickness of the UI. |
| `SlantField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How beveled the UI is. |
| `SpacingRatioField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How to space out the center UI and its buttons. |
| `TrackRatioField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the slider track should be compared to the UI. |
| `ButtonRatioField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the buttons should be compared to the slider. |
| `_trackMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[MultiBevelStripeMesh](https://wiki.resonite.com/Component:MultiBevelStripeMesh "Component:MultiBevelStripeMesh")** | The mesh for the slider track. |
| `_leftMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh for the left button. |
| `_rightMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh for the right button. |
| `_cursorMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh for the slider cursor. |
| `_trackMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the slider track. |
| `_leftMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the left button. |
| `_rightMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the right button. |
| `_cursorMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the slider cursor. |
| `_leftPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the left button. |
| `_rightPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the right button. |
| `_cursorPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the cursor. |
| `_leftColliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size field of the left button's collider. |
| `_rightColliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size field of the right button's collider. |
| `_trackColliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size field of the track's collider. |
| `_cursorColliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size field of the cursor's collider. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `LeftOnTouch:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the left button is touched. |
| `RightOnTouch:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the right button is touched. |

Triggers
Collapse

## Usage

Just dont.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacySlider&oldid=99058](https://wiki.resonite.com/index.php?title=Component:LegacySlider&oldid=99058)"

Contents