# Component:StaticSavedObjectProvider

> Source: https://wiki.resonite.com/Component:StaticSavedObjectProvider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6f/StaticSavedObjectProviderComponent.png/510px-StaticSavedObjectProviderComponent.png)](https://wiki.resonite.com/File:StaticSavedObjectProviderComponent.png) **Static Saved Object Provider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Not currently usable.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | Enter the Uri (e.g. resrec:///) link of the saved object |
| `PreGather` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to pregather the object's assets or not. |

Fields
Collapse

## Usage

> Unfortunately there's not a direct way to use it right now. The only usage is to pre-download some objects and their assets so they load faster, but I don't think we're actively using it even internally at this moment.
>
> It's an old thing that has been added in the past, but I forget the exact reason.
>
> —Answer from [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") from issue #2582 of a previous [FrooxEngine](https://wiki.resonite.com/FrooxEngine "FrooxEngine")-based application.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticSavedObjectProvider&oldid=95679](https://wiki.resonite.com/index.php?title=Component:StaticSavedObjectProvider&oldid=95679)"

Contents