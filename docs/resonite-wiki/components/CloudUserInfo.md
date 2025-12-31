# Component:CloudUserInfo

> Source: https://wiki.resonite.com/Component:CloudUserInfo

The CloudUserInfo component can be used to retrieve information about a user from the Resonite cloud, such as their name or profile picture, based on their user ID.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UserId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The ID of the user that this component should display information about |
| `IsLoaded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the given user's information has been loaded |
| `Username` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the given user |
| `RegistrationDate` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The time that the given user registered their account |
| `OriginalRegistrationDate` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The time that the given user registered their account which they [migrated](https://wiki.resonite.com/Migrations "Migrations") from. |
| `IconURL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | A URL, pointing to the user's profile picture |
| `IsContact` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not this user is one of your contacts (only works in [userspace](https://wiki.resonite.com/Userspace "Userspace")) |
| `_loadedUserId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The user ID corresponding to the information this component is currently outputting. This is an internal value and shouldn't be edited manually. |

Fields
Collapse

## Usage

To get info about a user, type their user ID into the `UserId` field of the component.

You can get their user ID through multiple ways, for example using the Protoflux node or Resonite's cloud API.

## Examples

Any item that populates an image with your profile icon and the default Profile Facet that is on your home dash tab with a new account.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CloudUserInfo&oldid=78700](https://wiki.resonite.com/index.php?title=Component:CloudUserInfo&oldid=78700)"

Contents