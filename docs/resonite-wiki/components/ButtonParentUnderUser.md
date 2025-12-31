# Component:ButtonParentUnderUser

> Source: https://wiki.resonite.com/Component:ButtonParentUnderUser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4e/ButtonParentUnderUserComponent.png/510px-ButtonParentUnderUserComponent.png)](https://wiki.resonite.com/File:ButtonParentUnderUserComponent.png) **Button Parent Under User** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonParentUnderUser** component takes in a [slot](https://wiki.resonite.com/Slot "Slot") and some optional parameters for parenting slots. When a [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed, this component will parent any slot provided to the user that pressed the button.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The [slot](https://wiki.resonite.com/Slot "Slot") to parent to the user that pressed the button. |
| `FindObjectRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Looks upwards in the slot heirarchy to find the slot with the [Object Root](https://wiki.resonite.com/Component:ObjectRoot "Component:ObjectRoot") component, and then parents that slot instead to the user. |
| `UnparentWhenParented` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this component's parenting effects togglable. |
| `PreserveOriginalSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Keep track of the original space. |
| `_originalSpace` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that represents the original space. |

Fields
Collapse

## Usage

Useful if you want certain slots to be parented to you when a button is pressed.

## Examples

This is seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector"), [ProtoFlux Node Browser](https://wiki.resonite.com/ProtoFlux_Node_Browser "ProtoFlux Node Browser"), and other menus with a button that has a pin icon.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonParentUnderUser&oldid=90356](https://wiki.resonite.com/index.php?title=Component:ButtonParentUnderUser&oldid=90356)"

Contents