# Component:DelegateProxySource

> Source: https://wiki.resonite.com/Component:DelegateProxySource

Collapse **Component image**

[File:DelegateProxySource\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=DelegateProxySource%601Component.png "File:DelegateProxySource`1Component.png") **Delegate Proxy Source\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DelegateProxySource** component is used to make a [Button](https://wiki.resonite.com/Component:Button "Component:Button") [UIX](https://wiki.resonite.com/UIX "UIX") element give a sync delegate proxy when grabbed. To use almost any sync delegate with this component, provide "Delegate" as the type.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Delegate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **T** | The field to proxy when grabbing. |

Fields
Collapse

## Usage

Attach to a slot with a valid [UIX](https://wiki.resonite.com/UIX "UIX") [Button](https://wiki.resonite.com/Component:Button "Component:Button") and provide a delegate to proxy. When the area is grabbed, the user will have the delegate in their hand.

## Examples

The delegate names under [Component:StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D").

## See Also

- [Sync Delegates](https://wiki.resonite.com/Sync_Delegates "Sync Delegates")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DelegateProxySource&oldid=96447](https://wiki.resonite.com/index.php?title=Component:DelegateProxySource&oldid=96447)"

Contents