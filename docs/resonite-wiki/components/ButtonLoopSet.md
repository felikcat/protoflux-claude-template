# Component:ButtonLoopSet

> Source: https://wiki.resonite.com/Component:ButtonLoopSet

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/ButtonLoopSetComponent.png/510px-ButtonLoopSetComponent.png)](https://wiki.resonite.com/File:ButtonLoopSetComponent.png) **Button Loop Set** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonLoopSet** component takes in an [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"). When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is in the same [slot](https://wiki.resonite.com/Slot "Slot"), it will set the loop on this playable media depending on what is set up in this component.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Playback` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | The referenced playable media. |
| `OnPress` | **[LoopSetOptions](https://wiki.resonite.com/Type:LoopSetOptions "Type:LoopSetOptions")** | Sets the type of loop for this media when pressed. |
| `OnRelease` | **[LoopSetOptions](https://wiki.resonite.com/Type:LoopSetOptions "Type:LoopSetOptions")** | Sets the type of loop for this media when released. |

Fields
Collapse

## Usage

Basically a loop button that can be setup anywhere.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonLoopSet&oldid=90372](https://wiki.resonite.com/index.php?title=Component:ButtonLoopSet&oldid=90372)"

Contents