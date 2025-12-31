# Component:LegacyButton

> Source: https://wiki.resonite.com/Component:LegacyButton

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/97/LegacyButtonComponent.png/510px-LegacyButtonComponent.png)](https://wiki.resonite.com/File:LegacyButtonComponent.png) **Legacy Button** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyButton** component is a leftover Component from content migrated from other platforms. It should not be used, and should be replaced whenever possible.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the button. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the button. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the button. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick the button is. |
| `Slant` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much Bevel the button should have. |
| `IsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `Pressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The Sync delegate to call when this button is pressed. |
| `Pressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The Sync delegate to call per engine update as this button is being held down. |
| `Released` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | The Sync delegate to call when this button has stopped being pressed. |
| `IsPressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the button is being pressed currently. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this button accepts interaction if the user isn't looking at it. |
| `_textSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the text visual for this button. |
| `_textRenderer` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer for this button. |
| `_buttonPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field for this button for physical pressing. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider size field for this button's collider. |
| `_colliderOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider offset field for this button's collider. |
| `_textPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The text position field for this button's text |
| `_textBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The 2d bounds of this button's text |
| `_holderMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh that is containing this button (like a parent UI. |
| `_buttonMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The Bevel mesh that makes up this button's visual. |
| `_holderMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of the parent UI mesh. |
| `_buttonMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material of this button's mesh visual |
| `_pressDepth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the user is currently pressing the button physically |
| `_flashIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How much to add to the emission of the holder material. |

Fields
Collapse

## Usage

Just no.

## Examples

Old content that has a yellow color schema.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyButton&oldid=99009](https://wiki.resonite.com/index.php?title=Component:LegacyButton&oldid=99009)"

Contents