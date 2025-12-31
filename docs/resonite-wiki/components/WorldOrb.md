# Component:WorldOrb

> Source: https://wiki.resonite.com/Component:WorldOrb

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:WorldOrb&diff=113778) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is about the WorldOrb [Component](https://wiki.resonite.com/Component "Component"), for usage on the in game item see: [World Orb](https://wiki.resonite.com/World_Orb "World Orb").


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2c/WorldOrbComponent.png/510px-WorldOrbComponent.png)](https://wiki.resonite.com/File:WorldOrbComponent.png) **World Orb** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SessionStartingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that started the session if this is a session orb. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The session or world this goes to. |
| `ActiveSessionURLs` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | A list of currently active sessions for the worldmm. |
| `CreateIfNotExists` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[WorldCreator](https://wiki.resonite.com/index.php?title=Type:WorldCreator&action=edit&redlink=1 "Type:WorldCreator (page does not exist)")** | A sync delegate to call when a session does not exist for the world for this world orb. Passes this component as an argument. |
| `OpenActionOverride` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <WorldOrb>** | The Sync delegate to call as an override for this world orb's open Action. Passes this component as an argument. |
| `Visit` | **[WorldOrb.VisitState](https://wiki.resonite.com/Component:WorldOrb#VisitState)** | Whether the local user has visted the target world. |
| `ActiveUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many active users are in the target world. |
| `RecordStateUpdated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the world orb has up to date info after spawn. |
| `IsPublic` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the world is public. |
| `CanModify` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the world can be modified and saved. |
| `LongPressIndicatorColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use when the world orb is long pressed. |
| `LongPressTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the user has to click to trigger a long press. |
| `_longPressIndicator` | **[RingMesh](https://wiki.resonite.com/Component:RingMesh "Component:RingMesh")** | The mesh that fills a ring indicator when doing a long press. |
| `_longPressIndicatorMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material used to indicate a long press. |
| `Touched` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") <WorldOrb, [TouchEventInfo](https://wiki.resonite.com/index.php?title=Type:TouchEventInfo&action=edit&redlink=1 "Type:TouchEventInfo (page does not exist)") >** | The Sync delegate to trigger when this world orb is touched. Sends this component and the touch info as arguments to the Sync Delegate. |
| `LongPressTriggered` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <WorldOrb>** | The Sync delegate to trigger when long pressing. Passes this component as an argument to the Sync delegate. |
| `_lastFetchedUrl` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The last URL fetched for this world. |
| `_isReadOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The target world is a read only world, no saving. |
| `_orbRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot storing the world orb visual. |
| `_infoRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot storing the text visual for information about the world. |
| `_thumbTex` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The texture being used to store the picture of the 360 session preview |
| `_thumbMaterial` | **[Projection360Material](https://wiki.resonite.com/Component:Projection360Material "Component:Projection360Material")** | The material making the inner world preview/session 360 picture. |
| `_shellMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material making a rim lighting around the world orb. |
| `_nameText` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer showing the name of the world. |
| `_creatorText` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer showing the name of the creator of the world. |
| `_visitsText` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer showing the current world visits number. |
| `_usersText` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer showing the current users number. |
| `_namePosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the position of the world name text. |
| `_creatorPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the position of the creator name text. |
| `_visitsPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the position of the visits amount. |
| `_usersPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the position of the user count text. |
| `_userCountText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with the world orb's world user count. |
| `_sizeDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the world orb's scale. |
| `_iconSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the icon visual. |
| `_iconTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The icon texture for this world orb's icon. |
| `_iconMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The Unlit Material for showing the icon. |
| `_iconPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the position of the world icon. |
| `_sessionStartDialog` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [NewWorldDialog](https://wiki.resonite.com/Component:NewWorldDialog "Component:NewWorldDialog") >** | The current dialogue for starting a new session |
| `_lastTouch` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The last time in world time that a user touched the orb. |
| `_lastFlash` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The last time in world time that a user double clicked the orb. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``CustomWorldStart:Action`1<NewWorldDialog>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [NewWorldDialog](https://wiki.resonite.com/Component:NewWorldDialog "Component:NewWorldDialog") >** | ✓ | Handles when the user asks to open a custom world. |
| `OnStartNewSession:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user starts a new session with default settings. |
| `OnStartCustomSession:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to open a custom session. |
| `OnJoinSession:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when a user joins the target session. |
| `OnEditMetadata:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when a user asks to edit the metadata. |
| `OnCancelMenu:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user cancels an action in a menu. |
| `OnCloneWorld:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to make a clone of the world. |
| `OnDeleteWorld:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to delete a world. |
| `OnReallyDeleteWorld:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to truely delete a world. |
| ``OnOverwrite:ButtonEventHandler`1<WorldOrb>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") <WorldOrb>** | ✓ | Handles when the user does a save overwrite. |

Triggers
Collapse

## VisitState

| Name | Value | Description |
| --- | --- | --- |
| `Visited` | 0 | The user has visited the world before, and there are no new updates. |
| `Updated` | 1 | The user has visited the world before, but it has been updated since then. |
| `New` | 2 | The user has never visited the target world. |

Values

## Usage

See [World Orb](https://wiki.resonite.com/World_Orb "World Orb").

## Examples

See [World Orb](https://wiki.resonite.com/World_Orb "World Orb") page for a picture of one.

## See Also

- [World Orb](https://wiki.resonite.com/World_Orb "World Orb")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldOrb&oldid=113778](https://wiki.resonite.com/index.php?title=Component:WorldOrb&oldid=113778)"

Contents