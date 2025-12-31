# Component:WorldCloseAction

> Source: https://wiki.resonite.com/Component:WorldCloseAction

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/46/WorldCloseActionComponent.png/510px-WorldCloseActionComponent.png)](https://wiki.resonite.com/File:WorldCloseActionComponent.png) **World Close Action** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldCloseAction** component is used to handle the leaving of a world after the user confirms leaving. This component only works on user space.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Action` | **[WorldCloseAction.CloseAction](https://wiki.resonite.com/Component:WorldCloseAction#CloseAction)** | The kind of action this [Button Events](https://wiki.resonite.com/Button_Events "Button Events") recieving Component is doing to a world. |
| `WaitingConfirm` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the game is waiting on confirmation via double click, which is 2 clicks within a 2 second time frame. |
| `OnClosed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | What Action Sync delegate to call when the world finishes closing. |

Fields
Collapse

## CloseAction

| Name | Value | Description |
| --- | --- | --- |
| `LeaveOrOpenCloseScreen` | 0 | This button is set to leave the world or open the save and close screen. |
| `Discard` | 1 | The user has opted to Discard the changes to the world and exit. |
| `Save` | 2 | The user has opted to save the changes to the world and then exit. |
| `SaveAs` | 3 | The user has opted to save the changes to the world, and specify a place to save the world orb before closing. |

Values

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the worlds browser for a user to leave a selected world.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldCloseAction&oldid=97828](https://wiki.resonite.com/index.php?title=Component:WorldCloseAction&oldid=97828)"

Contents