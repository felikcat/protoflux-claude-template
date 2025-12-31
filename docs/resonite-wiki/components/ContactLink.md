# Component:ContactLink

> Source: https://wiki.resonite.com/Component:ContactLink

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ContactLink&diff=113722) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/ContactLinkComponent.png/510px-ContactLinkComponent.png)](https://wiki.resonite.com/File:ContactLinkComponent.png) **Contact Link** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ContactLink** component allows a [slot](https://wiki.resonite.com/Slot "Slot") to be clicked on by a [user](https://wiki.resonite.com/User "User") to open their [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu") to the [Contacts Menu](https://wiki.resonite.com/Contacts_Menu "Contacts Menu") of a specific user (by using a provided `UserId`).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UserId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The [User ID](https://wiki.resonite.com/User_ID "User ID") of the User whose contact page will be opened upon clicking the object. |

Fields
Collapse

## Usage

Add the ContactLink component to an object, clicking on that object will open up the [Contacts Menu](https://wiki.resonite.com/Contacts_Menu "Contacts Menu") and will show the User page of the user defined in the `UserId` field. When you attach it, your own [User ID](https://wiki.resonite.com/User_ID "User ID") will be automatically filled in.

For [UIX](https://wiki.resonite.com/UIX "UIX"), a [button](https://wiki.resonite.com/Component:Button "Component:Button") component is required to click and take the user to that contact page. Otherwise, a collider works just fine without a button for this component to work.

## Examples

This is the component that allows Users to click on the [Nameplate](https://wiki.resonite.com/Nameplate "Nameplate") of another user and open their contact page quickly. You can find an example on by selecting your own nameplate and viewing the components

## See Also

On the default nameplate, a [AvatarNameTagAssigner](https://wiki.resonite.com/Component:AvatarNameTagAssigner "Component:AvatarNameTagAssigner") is set up to write the current user's [User ID](https://wiki.resonite.com/User_ID "User ID") to the ContactLink UserId field.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContactLink&oldid=113722](https://wiki.resonite.com/index.php?title=Component:ContactLink&oldid=113722)"

Contents