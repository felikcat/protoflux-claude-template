# Component:ContextMenu

> Source: https://wiki.resonite.com/Component:ContextMenu

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/ContextMenuComponent.png/510px-ContextMenuComponent.png)](https://wiki.resonite.com/File:ContextMenuComponent.png) **Context Menu** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ContextMenu** component is the main component that handles the functionality of every user's [Context Menu](https://wiki.resonite.com/Context_Menu "Context Menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Owner` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that is using this context menu |
| `Pointer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot that represents the pointer the user is interacting with the menu with. |
| `Separation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many degrees of separation each arc button has. |
| `LabelSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of image labels on the buttons |
| `RadiusRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ratio of the button arcs vs the size of the circle in the middle. |
| `_currentSummoner` | _direct_ **[SyncRef](https://wiki.resonite.com/Type:SyncRef "Type:SyncRef")** | The thing opening the menu currently |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The UIX canvas rendering the buttons. |
| `_arcLayout` | **[ArcLayout](https://wiki.resonite.com/Component:ArcLayout "Component:ArcLayout")** | The layout being used to arrange the buttons |
| `_canvasActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The active field of the canvas this context menu's visuals are being drawn on. |
| `_colliderEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The active field of the collider of the context menu to allow interaction with it. |
| `_iconImage` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The icon of the center circle button. Used to display the image of the hovered button option. |
| `_separation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field used to control the separation of button options in the context menu. |
| `_offsetMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset min field of the radial menu section |
| `_offsetMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset max field of the radial menu section. |
| `_innerCircle` | **[OutlinedArc](https://wiki.resonite.com/Component:OutlinedArc "Component:OutlinedArc")** | The graphic of the inner circle for the context menu |
| `_innerCircleButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button part of the inner circle of the context menu. |
| `_innerCircleAnchorMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The anchor min field of the rectangle transform of the inner circle graphic. Used to control how it looks when flicking and changing its size. |
| `_innerCircleAnchorMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The anchor max field of the rectangle transform of the inner circle graphic. Used to control how it looks when flicking and changing its size. |
| `_itemsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot that contains all the arc items that makes up the context menu options. |
| `_arcMaterial` | **[UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment")** | The material used to draw the menu options in the context meny. |
| `_fontMaterial` | **[UI\_TextUnlitMaterial](https://wiki.resonite.com/Component:UI_TextUnlitMaterial "Component:UI TextUnlitMaterial")** | The material used to render the text for the context menu options |
| `_spriteMaterial` | **[UI\_UnlitMaterial](https://wiki.resonite.com/Component:UI_UnlitMaterial "Component:UI UnlitMaterial")** | The material used to render the image sprites on the buttons in the context menu. |
| `_arcOverlay` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enable Overlay mode on the arc material. Used to control if the context menu should appear ontop of everything else. |
| `_fontOverlay` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enable Overlay mode on the font material. Used to control if the context menu should appear ontop of everything else. |
| `_spriteOverlay` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enable Overlay mode on the sprite material. Used to control if the context menu should appear ontop of everything else. |
| `_arcZTest` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | the Ztest field on the arc material. Used to control if the context menu should appear ontop of everything else. |
| `_fontZTest` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | the Ztest field on the font material. Used to control if the context menu should appear ontop of everything else. |
| `_spriteZTest` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ZTest](https://wiki.resonite.com/Type:ZTest "Type:ZTest")** | the Ztest field on the spite material. Used to control if the context menu should appear ontop of everything else. |
| `_zwriteArc` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | the Zwrite field on the arc material. Used to control if the context menu should appear ontop of everything else. |
| `_zwriteText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ZWrite](https://wiki.resonite.com/Type:ZWrite "Type:ZWrite")** | the Zwrite field on the font material. Used to control if the context menu should appear ontop of everything else. |
| `_arcRenderQueue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | the render queue field on the arc material. Used to control if the context menu should appear ontop of everything else. |
| `_fontRenderQueue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | the render queue field on the font material. Used to control if the context menu should appear ontop of everything else. |
| `_spriteRenderQueue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | the render queue field on the sprite material. Used to control if the context menu should appear ontop of everything else. |
| `_canvasOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Used to control if the context menu should appear ontop of everything else. |
| `_fillFade` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Is faded by `_lerp`. |
| `_outlineFade` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Is faded by `_lerp`. |
| `_textFade` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Is faded by `_lerp`. |
| `_iconFade` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Is faded by `_lerp`. |
| `_lerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Lerps between 0 and 1. 0 for context menu closed and 1 for context menu open. |
| `_state` | **[ContextMenu.State](https://wiki.resonite.com/Component:ContextMenu#State)** | Communicates what opening stage the context menu is in. |
| `_flickModeActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the context menu currently is being flicked. |
| `_flickEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the context menu currently allows flicking. |
| `_hidden` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the context menu is currently hidden from every user except `Owner` |
| `_selectedItem` | **[ContextMenuItem](https://wiki.resonite.com/Component:ContextMenuItem "Component:ContextMenuItem")** | The item currently being hovered over by the user's pointer. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `CloseMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Closes the menu if it is currently open. |
| `OnInnerPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the context menu inner circle is pressed. |
| `OnInnerReleased:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the context menu inner circle is released. |

Triggers
Collapse

## State

| Name | Value | Description |
| --- | --- | --- |
| `Closed` | 0 | The menu is currently closed. |
| `Opening` | 1 | The menu is doing it's opening animation. |
| `Opened` | 2 | The menu is fully open. |

Values

## See Also

- [Context Menu](https://wiki.resonite.com/Context_Menu "Context Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContextMenu&oldid=98764](https://wiki.resonite.com/index.php?title=Component:ContextMenu&oldid=98764)"

Contents