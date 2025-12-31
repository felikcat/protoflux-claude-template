# Component:ButtonOpenHome

> Source: https://wiki.resonite.com/Component:ButtonOpenHome

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b8/ButtonOpenHomeComponent.png/510px-ButtonOpenHomeComponent.png)](https://wiki.resonite.com/File:ButtonOpenHomeComponent.png) **Button Open Home** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonOpenHome** component, when pressed with an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton"), takes the [User](https://wiki.resonite.com/User "User") to their favorite home [world](https://wiki.resonite.com/World "World") (usually the [Resonite Cloud Home](https://wiki.resonite.com/Resonite_Cloud_Home "Resonite Cloud Home") by default). There is an optional [string](https://wiki.resonite.com/Type:String "Type:String") input for a [group home](https://wiki.resonite.com/Homes#Group_Home "Homes").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LastOpened` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | Shows when the world was last opened (not shown in the component). |
| `GroupOwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | An optional [string](https://wiki.resonite.com/Type:String "Type:String") input for a [group home](https://wiki.resonite.com/Homes#Group_Home "Homes"). |

Fields
Collapse

## Usage

This is an easy way to set up a way to get to your favorite home faster.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonOpenHome&oldid=90376](https://wiki.resonite.com/index.php?title=Component:ButtonOpenHome&oldid=90376)"

Contents