# Component:ButtonReferenceSet

> Source: https://wiki.resonite.com/Component:ButtonReferenceSet

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonReferenceSet&diff=90360) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/63/ButtonReferenceSet%601Component.png/510px-ButtonReferenceSet%601Component.png)](https://wiki.resonite.com/File:ButtonReferenceSet%601Component.png) **Button Reference Set\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonReferenceSet** component takes in a [Reference Type](https://wiki.resonite.com/Reference_Type "Reference Type") and a `TargetReference`. When an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") is pressed while this component is on the same [slot](https://wiki.resonite.com/Slot "Slot"), this will send the reference to the provided `TargetReference`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>** | The target to send the reference outwards. |
| `SetReference` | **T** | The reference to set when the button is pressed. |

Fields
Collapse

## Usage

This is similar to the [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node but as a component instead.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonReferenceSet&oldid=90360](https://wiki.resonite.com/index.php?title=Component:ButtonReferenceSet&oldid=90360)"

Contents