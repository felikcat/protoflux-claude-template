# Component:ObjectRoot

> Source: https://wiki.resonite.com/Component:ObjectRoot

Collapse **Component image**

[File:ObjectRootComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ObjectRootComponent.png "File:ObjectRootComponent.png") **Object Root** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ObjectRoot** component marks a [slot](https://wiki.resonite.com/Slot "Slot") as the root of an object, where an object is the slot itself plus all of its child slots, recursively.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `RemoveChildrenObjectRoots:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | will recursively delete any ObjectRoot components from this slot's children. |
| ``RemoveChildrenObjectRoots:Func`1<Int>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | X | will recursively delete any ObjectRoot components from this slot's children. |

Triggers
Collapse

## Usage

Setting a slot as the ObjectRoot helps the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")'s "up to object root" button find the root of the object.

## Examples

## See Also

## Related ProtoFlux nodes

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ObjectRoot&oldid=99083](https://wiki.resonite.com/index.php?title=Component:ObjectRoot&oldid=99083)"

Contents