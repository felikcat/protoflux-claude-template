# Component:SessionControlDialog

> Source: https://wiki.resonite.com/Component:SessionControlDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:SessionControlDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SessionControlDialogComponent.png "File:SessionControlDialogComponent.png") **Session Control Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SessionControlDialog** component is used to edit and view session settings like permissions, roles, and name to list a few.

See [Session](https://wiki.resonite.com/Session "Session").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ActiveTab` | **[SessionControlDialog.Tab](https://wiki.resonite.com/Component:SessionControlDialog#Tab)** | The tab this view is currently on. |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to place visuals for session options. |
| `_worldName` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field containing the session name. |
| `_maxUsers` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | The field containing the session max users. |
| `_awayKickEnabled` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The field containing the session away kick enabler. |
| `_awayKickMinutes` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | The field containing the session away kick minutes. |
| `_autosaveEnabled` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The field containing the session auto save enabler. |
| `_autosaveMinutes` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | The field containing the session auto save minutes. |
| `_autocleanEnabled` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The field containing the session auto clean enabler. |
| `_autocleanMinutes` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | The field containing the session auto clean minutes. |
| `_mobileFriendly` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The field containing the session mobile friendly enabler. |
| `_hideFromListing` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The field containing the session hide from listing enabler. |
| `_description` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field containing the session description. |
| `_worldNameButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session name. |
| `_descriptionButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session description. |
| `_maxUsersButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session max users. |
| `_awayKickEnabledButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session away kick enabled status. |
| `_awayKickMinutesButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session away kick minutes. |
| `_autosaveEnabledButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session auto save enabled status. |
| `_autosaveMinutesButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session auto save minutes. |
| `_autocleanEnabledButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session auto clean enabled button. |
| `_autocleanMinutesButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session auto clean minutes. |
| `_mobileFriendlyButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session mobile friendly enabled status. |
| `_hideFromListingButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the session hide from listing enabled status. |
| `_permissionOverridesIndicator` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The element that shows how many user overrides are currently active for permissions |
| `_permissionOverridesButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that resets all user overrides for permissions. |
| `_getSessionOrb` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that gets the session orb. |
| `_getWorldOrb` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that gets the world orb. |
| `_editMode` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that enables edit mode for the local user. |
| `_copySessionURL` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that copies the session URL. |
| `_copyWorldURL` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that copies the world URL. |
| `_copyRecordURL` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that copies the record URL. |
| `_accessLevelRadios` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Radio](https://wiki.resonite.com/Type:Radio "Type:Radio")** | The set of radios to set session access level. |
| `_accessLevelRadiosButtons` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The set of radio buttons to set session access level. |
| `_worldNameSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field that is used to edit the world Name. |
| `_descriptionSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field that is used to edit the world description. |
| `_maxUsersSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The field that is used to edit the world max Users. |
| `_awayKickEnabledSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world away Kick Enabled. |
| `_awayKickMinutesSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field that is used to edit the world away Kick Minutes. |
| `_autosaveEnabledSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world auto save Enabled. |
| `_autosaveMinutesSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field that is used to edit the world auto save Minutes. |
| `_autocleanEnabledSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world auto clean Enabled. |
| `_autocleanSecondsSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field that is used to edit the world auto clean Seconds. |
| `_mobileFriendlySync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world mobile Friendly. |
| `_hideFromListingSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world hide From Listing. |
| `_editModeSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world edit Mode status for the local user. |
| `_accessLevelSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel") >** | The field that is used to edit the world access Level. |
| `_customVerifierLabel` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The label used to indicate the world's custom verifier. |
| `_customVerifierCheckbox` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | The checkbox for enabling/disabling a custom world verifier. |
| `_customVerifierButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for enabling/disabling a custom world verifier. |
| `_customVerifierSync` | **[WorldValueSync\`1](https://wiki.resonite.com/Component:WorldValueSync%601 "Component:WorldValueSync`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field that is used to edit the world custom Verifier. |
| `_uiContentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that contains all the ui content of the world. |
| `_slideSwap` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | The swap region used to make the animation for going between session menu views. |
| `_saveWorld` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to save world changes. |
| `_saveWorldAs` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to save the world as a certain name. |
| `_saveWorldCopy` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to save a copy of the world. |
| `_tabButtons` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | A list of the buttons used to change between session menu views. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SwitchTab:ButtonEventHandler`1<SessionControlDialog.Tab>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [SessionControlDialog.Tab](https://wiki.resonite.com/Component:SessionControlDialog#Tab) >** | ✓ | Called when a session menu tab button is touched. |
| `GetSessionOrb:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the get session orb button is touched. |
| `GetWorldOrb:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the get world orb button is touched. |
| `CopySessionURL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the copy session url button is touched. |
| `CopyWorldURL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the copy world url button is touched. |
| `CopyRecordURL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the copy record url button is touched. |
| `CustomVerifierPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the custom verifier button is touched. |
| `OnEnableCustomJoinVerifier:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the enable custom verifier button is touched. |
| `OnClearUserPermissionOverrides:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the clear custom permission overrides button is touched. |
| `OnSave:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the save world button is touched. |
| `OnSaveAs:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the save world as button is touched. |
| `OnSaveCopy:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the save world copy button is touched. |

Triggers
Collapse

## Tab

| Name | Value | Description |
| --- | --- | --- |
| `Settings` | 0 | The tab is currently on Session Settings. |
| `Users` | 1 | The tab is currently on Users. |
| `Permissions` | 2 | The tab is currently on Permissions. |

Values

## Usage

See [Session](https://wiki.resonite.com/Session "Session").

## Examples

See [Session](https://wiki.resonite.com/Session "Session").

## See Also

- [Session](https://wiki.resonite.com/Session "Session")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SessionControlDialog&oldid=99168](https://wiki.resonite.com/index.php?title=Component:SessionControlDialog&oldid=99168)"

Contents