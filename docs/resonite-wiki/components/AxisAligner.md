# Component:AxisAligner

> Source: https://wiki.resonite.com/Component:AxisAligner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AxisAligner&diff=97403) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/72/AxisAlignerComponent.png/510px-AxisAlignerComponent.png)](https://wiki.resonite.com/File:AxisAlignerComponent.png) **Axis Aligner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisAligner** component is used to Align elements along a single line axis in local space under a slot based on their Bounding boxes. It also allows for excluding bounded elements from calculations, and for aligning elements themselves so that they can be centered like varied sized beads on a string or like boxes into the corner edge between a wall and floor. These calculations are heavy, and this component is best used lightly. Remove this component after using it to Align world elements, as it will be constantly active and will behave violently if used to Align shelves for example in a world and left unremoved.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoAddChildren` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether slots below this component's slot in the hierarchy are automatically added to `_targets` |
| `AutoAddIgnoreTags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | if `AutoAddChildren` is enabled. A slot will not be added to `_targets` if it's tag is in this list. |
| `Direction` | **[AxisAligner.AxisDir](https://wiki.resonite.com/Component:AxisAligner#AxisDir)** | The axis and direction the items will be aligned on |
| `GlobalAxisXAlign` | **[AxisAligner.Align](https://wiki.resonite.com/Component:AxisAligner#Align)** | Controls how items will be aligned globally, with each other in the X Axis |
| `GlobalAxisYAlign` | **[AxisAligner.Align](https://wiki.resonite.com/Component:AxisAligner#Align)** | Controls how items will be aligned globally, with each other in the Y Axis |
| `GlobalAxisZAlign` | **[AxisAligner.Align](https://wiki.resonite.com/Component:AxisAligner#Align)** | Controls how items will be aligned globally, with each other in the Z Axis |
| `ElementAxisXAlign` | **[AxisAligner.Align](https://wiki.resonite.com/Component:AxisAligner#Align)** | Controls how each item aligns itself, within the align, in the X Axis |
| `ElementAxisYAlign` | **[AxisAligner.Align](https://wiki.resonite.com/Component:AxisAligner#Align)** | Controls how each item aligns itself, within the align, in the Y Axis |
| `ElementAxisZAlign` | **[AxisAligner.Align](https://wiki.resonite.com/Component:AxisAligner#Align)** | Controls how each item aligns itself, within the align, in the Z Axis |
| `Separation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The spacing between each item in `_targets` along the specified axis |
| `ExcludeList` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IBounded](https://wiki.resonite.com/Type:IBounded "Type:IBounded")** | A list of Bounded elements under target slots which are excluded from the aligners bounds calculations |
| `_targets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AxisAligner.Target](https://wiki.resonite.com/Component:AxisAligner#Target)** | A list of slots which will be aligned. This will be automatically generated if `AutoAddChildren` is enabled. |

Fields
Collapse

## Target

| Name | Type | Description |
| --- | --- | --- |
| `TargetSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to read bounds data from. |
| `PositionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of `TargetSlot` to drive in order to align it. |

Fields

## Align

Note: changing the alignment does not change the order of elements. Just how the bounding box for the elements is positioned relative to 0. Basically this acts as a translation alignment, rather than a reordering of elements.

| Name | Value | Description |
| --- | --- | --- |
| `Neg` | 0 | Align the elements on this axis starting at zero going towards the negative direction. |
| `Mid` | 1 | Align the elements on this axis so that the Bounded center ends up at 0 on this axis. |
| `Pos` | 2 | Align the elements on this axis starting at 0 going towards the positive direction. |

Values

## AxisDir

_This article or section is a stub. You can help the Resonite wiki by expanding it._

| Name | Value | Description |
| --- | --- | --- |
| `Xpos` | 0 | Align elements in a line towards the positive X axis locally. |
| `Xneg` | 1 | Align elements in a line towards the negative X axis locally. |
| `Ypos` | 2 | Align elements in a line towards the positive Y axis locally. |
| `Yneg` | 3 | Align elements in a line towards the negative Y axis locally. |
| `Zpos` | 4 | Align elements in a line towards the positive Z axis locally. |
| `Zneg` | 5 | Align elements in a line towards the negative Z axis locally. |

Values

## Disadvantages and Alternatives

As the Axis Aligner works off of Bounds Calculations, and runs its calculations under a wide range of criteria, it can quickly become heavy with a doezen slots or so. Its Bounds-based nature alao makes it unsuited for evenly spacing objects with different bounds.

To mitigate these kinds of issues, one can make their own version of this in Protoflux, by having OnChange or other triggers fire a ForLoop, which iterates through all Slot Children, and gives them an offset based on the Iteration multiplied by a Float3 for the position. To further implement the bounds functionality, one can use a value that increases by the bounds calculation every iteration, instead of a number based on the Iteration itself.

A simple example was used to align the Avatars in [Avatar Station](https://wiki.resonite.com/index.php?title=Avatar_Station&action=edit&redlink=1 "Avatar Station (page does not exist)"), and is available in Nuki's Public Folder.

## Examples

- [AxisAligner tutorial](https://www.youtube.com/watch?v=NkjcGAwlZMs) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisAligner&oldid=97403](https://wiki.resonite.com/index.php?title=Component:AxisAligner&oldid=97403)"

Contents