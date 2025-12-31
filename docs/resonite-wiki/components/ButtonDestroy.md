# Component:ButtonDestroy

> Source: https://wiki.resonite.com/Component:ButtonDestroy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3e/ButtonDestroyComponent.webp/510px-ButtonDestroyComponent.webp.png)](https://wiki.resonite.com/File:ButtonDestroyComponent.webp) **Button Destroy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonDestroy** component destroys the Target [IDestroyable](https://wiki.resonite.com/index.php?title=IDestroyable&action=edit&redlink=1 "IDestroyable (page does not exist)") on [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") interaction, such as a [slot](https://wiki.resonite.com/Slot "Slot").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[IDestroyable](https://wiki.resonite.com/Type:IDestroyable "Type:IDestroyable")** | The destroyable slot target. |
| `FindObjectRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When this is interacted, this component will take the target and go up in the hierarchy and look for the first [object root](https://wiki.resonite.com/Component:ObjectRoot "Component:ObjectRoot") slot, then destroys it. |

Fields
Collapse

## Usage

This can be used in projects that need things destroyed by a button press.

## Examples

The **ButtonDestroy** component can be found in many of the default interfaces such as the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonDestroy&oldid=90345](https://wiki.resonite.com/index.php?title=Component:ButtonDestroy&oldid=90345)"

Contents