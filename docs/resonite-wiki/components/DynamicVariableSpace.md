# Component:DynamicVariableSpace

> Source: https://wiki.resonite.com/Component:DynamicVariableSpace

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicVariableSpace&diff=92219) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/DynamicVariableSpaceComponent.png/510px-DynamicVariableSpaceComponent.png)](https://wiki.resonite.com/File:DynamicVariableSpaceComponent.png) **DynamicVariableSpace** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Introduction

The **DynamicVariableSpace** component is used to separate dynamic variables into namespaces.
Since dynamic variables are, by default, created on the slot of the nearest parent DynamicVariableSpace, this component provides control over where the root of that space is, as well as part of the path name to be referenced when using a consumer of dynamic variables, such as [DynamicValueVariableDriver\`1](https://wiki.resonite.com/DynamicValueVariableDriver%601_(Component) "DynamicValueVariableDriver`1 (Component)"). For more info see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables").

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Having multiple of these components (with the same space name) in the same hierarchy can cause unintended behaviour. If you're having issues with using this component, consider placing this higher in the hierarchy or avoid duplicating a slot that uses this component.


## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SpaceName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the space. |
| `OnlyDirectBinding` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When enabled, variables won't be bound to this space unless they specify it by name: <spacename>/<varname>. |

Fields
Collapse

## Behavior

## Examples

By default worlds have a DynamicVariableSpace named "World" and users have a DynamicVariableSpace named "User"

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicVariableSpace&oldid=92219](https://wiki.resonite.com/index.php?title=Component:DynamicVariableSpace&oldid=92219)"

Contents