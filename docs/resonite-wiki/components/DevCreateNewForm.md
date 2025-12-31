# Component:DevCreateNewForm

> Source: https://wiki.resonite.com/Component:DevCreateNewForm

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d1/DevCreateNewFormComponent.png/510px-DevCreateNewFormComponent.png)](https://wiki.resonite.com/File:DevCreateNewFormComponent.png) **Dev Create New Form** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OnCreated` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ItemCreated](https://wiki.resonite.com/index.php?title=Type:ItemCreated&action=edit&redlink=1 "Type:ItemCreated (page does not exist)")** | The Sync delegate to call when an item is created. |
| `CategoryRoot` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The current location in the create menu we are at. |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to list content like buttons and such. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``RunAction:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | See [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard"). |
| ``ReturnToCategory:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | See [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard"). |
| ``NestIntoCategory:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | See [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard"). |

Triggers
Collapse

## Usage

See [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard").

## Examples

See [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard").

## See Also

- [Create New Wizard](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DevCreateNewForm&oldid=98420](https://wiki.resonite.com/index.php?title=Component:DevCreateNewForm&oldid=98420)"

Contents