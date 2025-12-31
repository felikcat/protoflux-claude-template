# Component:Workspace

> Source: https://wiki.resonite.com/Component:Workspace

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/79/WorkspaceComponent.png/510px-WorkspaceComponent.png)](https://wiki.resonite.com/File:WorkspaceComponent.png) **Workspace** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

This component works in [Userspace](https://wiki.resonite.com/Userspace "Userspace") only, so a lot of it's features and potential is locked behind this. This is only used for saving the dash at the moment


The **Workspace** component allows for doing work inside of a containerized slot, where the user can add or remove items which gets saved every interval specified. These workspaces can be public or private, and work similarly in concept to [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables") except greatly simplified and store an entire hierarchy instead of a single value. Workspaces have a path to them, which allow for having multiple different workspaces per user. Workspaces take up storage as a saved item would, and automatically synchronize in real time. Multiple users working on workspaces at the same time can cause issues however, since workspaces save their changes before loading from the cloud unless `ReadOnly` is enabled.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to manage reading and writing the contents of this workspace to the cloud for. |
| `OverrideOwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The override for the owner of this workspace to read and write the data for, which allows for reading public workspaces from others. |
| `WorkspacePath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The path of the workspace on the Cloud. Adding "public/" (case ignored) to the start of the path allows for public workspaces anyone can edit. Public workspaces must exist first before another user than the owner can save to them. |
| `InitializeWorkspace` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | A [Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") to call that takes a slot for when this component generates the work space. the slot is the slot this component is on. |
| `ReadOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only read the contents of this workspace from the cloud and not save it. |
| `AutosaveDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long to wait between save attempts before trying to save again. saves only happen if there have been changes. |
| `SuspendUpdates` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to pause the loading and saving of this workspace to the cloud. |
| `_unsavedChanges` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this workspace has changes that should be saved to the cloud upon the next save. |
| `_lastModification` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The last time the workspace was changed. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnMarkModified:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Tells this component it's hiearchy is modified. Can also be done with the [Notify Modified](https://wiki.resonite.com/ProtoFlux:Notify_Modified "ProtoFlux:Notify Modified") Node on any element on or under this component's slot. |
| `OnSaveWorkspace:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Forces the workspace to save it's changes. |

Triggers
Collapse

## Behavior

## Examples

- This can be useful for users who want to work on the same thing, at different times.
- This can also be useful for keeping an object syncronized across multiple areas in a game, since it will load the same object into multiple different locations automatically.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Workspace&oldid=99052](https://wiki.resonite.com/index.php?title=Component:Workspace&oldid=99052)"

Contents