# Component:NewWorldDialog

> Source: https://wiki.resonite.com/Component:NewWorldDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9d/NewWorldDialogComponent.png/510px-NewWorldDialogComponent.png)](https://wiki.resonite.com/File:NewWorldDialogComponent.png) **New World Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NewWorldDialog** component is used internally to control the new world prompt when making a new world in dash space.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_worldName` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to define the name of the new world. |
| `_mobileFriendly` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether the new world should be mobile friendly. |
| `_unsafeMode` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether the new world is going to be unsafe mode. |
| `_autoPort` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether the new world should boot with auto defined port. |
| `_port` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The port of the new world. |
| `_accessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | The access level of the new world. |
| `CustomStart` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <NewWorldDialog>** | The Sync delegate to call, passing this Dialog upon the world being made. |
| `_presetIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Which preset to use for the new world. |
| `_uiBuilt` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the world UI is built. |
| `_accessLevelRadios` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[ValueRadio\`1](https://wiki.resonite.com/Component:ValueRadio%601 "Component:ValueRadio`1") < [SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel") >** | A list of session access level options for the UI. |
| `_initialized` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the UI is built and ready. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnStartSession:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the start session button is touched. |

Triggers
Collapse

## Usage

Used internally.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NewWorldDialog&oldid=105340](https://wiki.resonite.com/index.php?title=Component:NewWorldDialog&oldid=105340)"

Contents