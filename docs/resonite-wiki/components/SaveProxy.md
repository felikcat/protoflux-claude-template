# Component:SaveProxy

> Source: https://wiki.resonite.com/Component:SaveProxy

Collapse **Component image**

[File:SaveProxyComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SaveProxyComponent.png "File:SaveProxyComponent.png") **Save Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Save Proxy** component saves another slot instead of this one when the slot this component is on is saved.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to save the hiearchy of when the slot this component is on is saved instead of this slot. |

Fields
Collapse

## Usage

Can be used to make an item save an external slot or object without having to parent it first.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SaveProxy&oldid=101077](https://wiki.resonite.com/index.php?title=Component:SaveProxy&oldid=101077)"

Contents