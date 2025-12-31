# Component:ReferenceReceiver

> Source: https://wiki.resonite.com/Component:ReferenceReceiver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceReceiver&diff=98940) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c7/ReferenceReceiver%601Component.png/510px-ReferenceReceiver%601Component.png)](https://wiki.resonite.com/File:ReferenceReceiver%601Component.png) **Reference Receiver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceReceiver** component can receive a reference dropped onto a [UIX](https://wiki.resonite.com/UIX "UIX") element [Button](https://wiki.resonite.com/Component:Button "Component:Button") by a [user](https://wiki.resonite.com/User "User"). The reference dropped is then stored into the field specified by `TargetReference` (an example would be to use the [ReferenceField](https://wiki.resonite.com/Component:ReferenceField "Component:ReferenceField")).

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

This component has a non generic version of the same name. That component uses a " [ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef")" instead of " [ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef") < **T** >" for `TargetReference`.


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[ISyncRef](https://wiki.resonite.com/Type:ISyncRef "Type:ISyncRef")** | The target field to fill when a reference is received. |
| `Undoable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether dropping elements onto this UIX interactable is [undoable](https://wiki.resonite.com/Undo "Undo"). |

Fields
Collapse

## Usage

- Letting go when the reference you want to send into the `TargetReference` field, is currently the way on how it can trigger.
- Combining this with the [ReferenceProxySource](https://wiki.resonite.com/Component:ReferenceProxySource "Component:ReferenceProxySource") component is a powerful way of moving references around without the need to open a [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector"). Having a [ReferenceField](https://wiki.resonite.com/Component:ReferenceField "Component:ReferenceField") of [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") as the `TargetReference` is the most recommended way of successfully transferring a reference this way.

## Examples

This can be used to allow the user to put in slots, music, or even value fields in a [UIX](https://wiki.resonite.com/UIX "UIX") canvas/panel for installers/settings for different systems.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceReceiver&oldid=98940](https://wiki.resonite.com/index.php?title=Component:ReferenceReceiver&oldid=98940)"

Contents