# Component:ButtonWorldLink

> Source: https://wiki.resonite.com/Component:ButtonWorldLink

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/53/ButtonWorldLinkComponent.png/510px-ButtonWorldLinkComponent.png)](https://wiki.resonite.com/File:ButtonWorldLinkComponent.png) **Button World Link** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonWorldLink** component takes in a [WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink") Component. When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is in the same [slot](https://wiki.resonite.com/Slot "Slot") as it, this component will attempt to open a [world](https://wiki.resonite.com/World "World") that is provided from that world link component.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LastOpened` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | Shows the last opened time (not seen in the component). |
| `WorldLink` | **[WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink")** | The [WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink") component that contains the world information. |

Fields
Collapse

## Usage

This allows a user to make customizable world loading buttons, either as a way to go to another world or to pre-load a world.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonWorldLink&oldid=90366](https://wiki.resonite.com/index.php?title=Component:ButtonWorldLink&oldid=90366)"

Contents