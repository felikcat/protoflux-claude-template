# Component:InspectorMemberActions

> Source: https://wiki.resonite.com/Component:InspectorMemberActions

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c1/InspectorMemberActionsComponent.png/510px-InspectorMemberActionsComponent.png)](https://wiki.resonite.com/File:InspectorMemberActionsComponent.png) **Inspector Member Actions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InspectorMemberActions** component is used in inspectors to make the clicking on the left hand side button behavior that brings up a context menu.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Member` | **[ISyncMember](https://wiki.resonite.com/index.php?title=Type:ISyncMember&action=edit&redlink=1 "Type:ISyncMember (page does not exist)")** | The member to bring up a context menu with opens to break drives and a few other things. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ResetField:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Reset the field to the default value. |
| `BreakLinkDrive:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Set the driver target driving this field from this field to null. |
| `OpenLinkDriveSource:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Open the component driving this field. |
| `Normalize:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Normalize this value if it's a set of more than 1 value. |
| `SetAllToAvg:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Average the components of this value if it's a set of more than 1 value. |
| ``SetAllToComponent:ButtonEventHandler`1<Int>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Set all the components of this value to X component. |
| `BakeBlendshape:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Bake this blendshape if it's a blendshape. |
| `RemoveBlendshape:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Remove this blendshape if it's a blendshape. |
| `SplitBlendshapeX:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Split the blendshape along the X axis. |
| `SplitBlendshapeY:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Split the blendshape along the Y axis. |
| `SplitBlendshapeZ:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Split the blendshape along the Z axis. |

Triggers
Collapse

## Usage

Used possibly in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")
- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InspectorMemberActions&oldid=98461](https://wiki.resonite.com/index.php?title=Component:InspectorMemberActions&oldid=98461)"

Contents