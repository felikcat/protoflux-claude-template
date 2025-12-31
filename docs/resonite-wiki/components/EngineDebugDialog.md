# Component:EngineDebugDialog

> Source: https://wiki.resonite.com/Component:EngineDebugDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:EngineDebugDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=EngineDebugDialogComponent.png "File:EngineDebugDialogComponent.png") **Engine Debug Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **EngineDebugDialog** component is used in the debug screen of the dash to show debug information about the game at the current moment.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DisplayMode` | **[EngineDebugDialog.Mode](https://wiki.resonite.com/Component:EngineDebugDialog#Mode)** | How to display the content. |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Content of the debug dialouge. |
| `_text` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text displaying the engine debug info. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SwitchToGatherJobs:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Gather Jobs one. |
| `SwitchToWorlds:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Worlds one. |
| `SwitchToLoadedAssets:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Loaded Assets one. |
| `SwitchToSpecial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Special one. |
| `SwitchToFocusedWorld:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Focused World one. |
| `SwitchToPhysics:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Physics one. |
| `SwitchToBackgroundJobs:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the dialog screen to the Background Jobs one. |
| `CapturePerformanceStats:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Copies the performance stats to the clipboard. |
| `UploadCC0Textures:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | DEVELOPER TEAM ONLY. DOES NOT DO ANYTHING ON PUBLIC BUILDS! |
| `CopyBackgroundWorkerSnapshot:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Copies a background worker snapshot to disk. |
| `StartRecordingPerfMetrics:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Records performance metrics to disk. |
| `ForceFullGC:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Forces the engine to garbage collect all ram data. |
| `SaveObjectPoolStats:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Saves object pool stats to disk. |
| `SwitchToNormalDash:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Closes the dialog. |

Triggers
Collapse

## Mode

[Template:Table EnumFields](https://wiki.resonite.com/index.php?title=Template:Table_EnumFields&action=edit&redlink=1 "Template:Table EnumFields (page does not exist)")

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EngineDebugDialog&oldid=98813](https://wiki.resonite.com/index.php?title=Component:EngineDebugDialog&oldid=98813)"

Contents