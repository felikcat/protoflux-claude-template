# Component:DestroyProxy

> Source: https://wiki.resonite.com/Component:DestroyProxy

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DestroyProxy&diff=91227) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fe/DestroyProxyComponent.png/510px-DestroyProxyComponent.png)](https://wiki.resonite.com/File:DestroyProxyComponent.png) **Destroy Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DestroyTarget` | **[IDestroyable](https://wiki.resonite.com/Type:IDestroyable "Type:IDestroyable")** | The slot, component (etc) to destroy. |

Fields
Collapse

## Usage

The DestroyProxy component is used to automatically destroy a specified `DestroyTarget` when this component itself or it's parent slot is destroyed.

Important to note: If you'd like to remove the component, first unset the `DestroyTarget` or else the target IDestroyable object will be destroyed as well.

## Examples

This can be put under a slot with a bunch of other destroy proxies that group together certain feature sets on an avatar, item or world. When the slot is destroyed, every destroy proxy on the slot will destroy everything they point to. This is useful for example, making multiple avatars with different feature sets and removing them to make simpler versions.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DestroyProxy&oldid=91227](https://wiki.resonite.com/index.php?title=Component:DestroyProxy&oldid=91227)"

Contents