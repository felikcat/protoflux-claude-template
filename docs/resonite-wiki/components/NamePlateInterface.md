# Component:NamePlateInterface

> Source: https://wiki.resonite.com/Component:NamePlateInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dc/NamePlateInterfaceComponent.png/510px-NamePlateInterfaceComponent.png)](https://wiki.resonite.com/File:NamePlateInterfaceComponent.png) **Name Plate Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NamePlateInterface** component is a [favoritable](https://wiki.resonite.com/Favorites "Favorites") type component that allows a user to set their custom nameplate for avatars they spawn into

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component is currently unimplemented. Source code structures indicate no references to this component. The nameplate system as it is has several issues on the issue tracker. This will most likely be implemented along with many nameplate bug fixes in the """contacts and profiles update""" milestone.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The name of this dialogue |
| `SpawningUser` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that spawned the dialouge |
| `SpawningUserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field containing the User ID of the person that spawned the dialogue |
| `IsInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this dialogue was spawned by the game (true) or spawned from inventory (false) |
| `Username` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to set with the username of the user who this nameplate has been spawned onto. |
| `UserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to set with the UserID of the user who this nameplate has been spawned onto. |
| `IconURL` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | The field to set with the User profile icon of the user who this nameplate has been spawned onto. |
| `TargetUser` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [User](https://wiki.resonite.com/Type:User "Type:User") >** | The field to set with the user this nameplate has been spawned onto. |
| `TargetUserRef` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | A user reference block to store info about the user this nameplate has been spawned onto. |
| `VoiceStream` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource") >** | The field to populate with the user voice stream of the user this nameplate has been spawned onto. |

Fields
Collapse

## Usage

Currently unimplemented.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- Component:NamePlateInterface
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NamePlateInterface&oldid=95721](https://wiki.resonite.com/index.php?title=Component:NamePlateInterface&oldid=95721)"

Contents