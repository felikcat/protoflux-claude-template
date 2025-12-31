# Component:BooleanSwitcher

> Source: https://wiki.resonite.com/Component:BooleanSwitcher

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BooleanSwitcher&diff=98334) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/45/BooleanSwitcherComponent.png/510px-BooleanSwitcherComponent.png)](https://wiki.resonite.com/File:BooleanSwitcherComponent.png) **Boolean Switcher** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The BooleanSwitcher component can be used to enable and disable a list of Slots depending on an index in the list.
It does so by driving the Active field of the slots.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoAddChildren` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, the Targets list will be automatically populated with the child slots of the slot that this component is on. |
| `AutoAddIgnoreTags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Don't auto add a child slot to the list if it has a tag that is in this list. |
| `Targets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The list of slots of which one will be enabled. |
| `ActiveIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The index of the currently active slot. |
| `ActivationMode` | **[BooleanSwitcher.Mode](https://wiki.resonite.com/Component:BooleanSwitcher#Mode)** | Allows for enabling items in `Target` based on `ActiveIndex` number. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetupForChildrenObjects:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Tells the boolean switcher to add all the children slot active fields of it's slot to it's list. |

Triggers
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `AtIndexOnly` | 0 | Activates only item at `ActiveIndex`. |
| `AllButIndex` | 1 | Activates all items except the one at `ActiveIndex` which will be disabled. |
| `IndexAndBefore` | 2 | Activates all items that are before and at `ActiveIndex`. |
| `IndexAndAfter` | 3 | Activates all items at and after `ActiveIndex` |

Values

## Usage

## Examples

- [BooleanSwitcher tutorial](https://www.youtube.com/watch?v=F0PhN-VxPEI) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime"). May be out of date.

## Related Issues

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanSwitcher&oldid=98334](https://wiki.resonite.com/index.php?title=Component:BooleanSwitcher&oldid=98334)"

Contents