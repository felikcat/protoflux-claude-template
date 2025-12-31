# Component:TextDisplayInterface

> Source: https://wiki.resonite.com/Component:TextDisplayInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c6/TextDisplayInterfaceComponent.png/510px-TextDisplayInterfaceComponent.png)](https://wiki.resonite.com/File:TextDisplayInterfaceComponent.png) **Text Display Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextDisplayInterface** component is used to specify what the user's favorite display of clipboard contents should be when pasting text not into a text field and the text is not a link.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The name of this favoritable item. |
| `SpawningUser` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that spawned this favoritable item. |
| `SpawningUserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field containing the ID of the user that spawned this favoritable item. |
| `IsInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this item was spawned by the player (false) or was spawned by the game as part of the favorites system (true). |
| `Heading` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with what the header text is upon spawn. |
| `Text` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with what the text the user pasted was upon spawn. |
| `RTF` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to fill with whether the text should be interpreted as Rich Text Format. This is usually the RTF field on a text rendering Component for the UI. |

Fields
Collapse

## Usage

Spawn the default resonite one from resonite essentials and edit it, or attach a new one and create a UI for it yourself. Once done, save to your inventory and set as your text display to make it your active one.

## Examples

The default Resonite text display in Resonite Essentials.

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- Component:TextDisplayInterface
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextDisplayInterface&oldid=95722](https://wiki.resonite.com/index.php?title=Component:TextDisplayInterface&oldid=95722)"

Contents