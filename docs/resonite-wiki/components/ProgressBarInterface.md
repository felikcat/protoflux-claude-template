# Component:ProgressBarInterface

> Source: https://wiki.resonite.com/Component:ProgressBarInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/49/ProgressBarInterfaceComponent.png/510px-ProgressBarInterfaceComponent.png)](https://wiki.resonite.com/File:ProgressBarInterfaceComponent.png) **Progress Bar Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProgressBarInterface** component is a [favoritable](https://wiki.resonite.com/Favorites "Favorites") item that appears when the user imports a file into Resonite.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The name of this favoritable interface. |
| `SpawningUser` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that spawned this favoritable interface. |
| `SpawningUserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field containing the ID of the user that spawned this favoritable interface. |
| `IsInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this interface is an instance. |
| `ProgressKnown` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to drive with whether or not the progress is known of the importing item. |
| `Progress` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to drive with the current progress import percentage from 0 to 1 of the importing item. |
| `ProcessedCountKnown` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to drive with whether or not the amount of processed items is known for the importing item. |
| `ProcessedItemCount` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The field to drive with the number of processed items for the importing item. |
| `TotalItemCountKnown` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to drive with whether the total number of items that need to be processed for the importing item is known. |
| `TotalItemCount` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The field to drive with the total number of items that need to be processed for the importing item. |
| `PhaseName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to drive with the current phase name of the importing item being imported is. |
| `SubPhaseName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to drive with the current sub phase name of the item being imported. |
| `Stage` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ProgressStage](https://wiki.resonite.com/Type:ProgressStage "Type:ProgressStage") >** | The field to drive with the progress stage for the importing item. |
| `HasCompleted` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to drive with whether the item has finished importing. |
| `HasFailed` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to drive with whether the item has failed to import. |
| `CompletionMessage` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to drive with the message for when the item has finished importing. |
| `FailureReason` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to drive with the failure reason for something to import. |
| `CanBeHidden` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to drive with whether this import dialogue can be hidden by the user. |

Fields
Collapse

## Usage

Used to make custom import dialogue visuals for a user by saving a custom UI with this component to inventory and setting as custom loading indicator.

## Examples

The default loading indicator visual in the resonite essentials example UI.

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- Component:ProgressBarInterface
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProgressBarInterface&oldid=95461](https://wiki.resonite.com/index.php?title=Component:ProgressBarInterface&oldid=95461)"

Contents