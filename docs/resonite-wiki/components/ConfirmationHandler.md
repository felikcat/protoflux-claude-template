# Component:ConfirmationHandler

> Source: https://wiki.resonite.com/Component:ConfirmationHandler

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ConfirmationHandler&diff=98350) which are not marked for translation.

Collapse **Component image**

[File:ConfirmationHandlerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ConfirmationHandlerComponent.png "File:ConfirmationHandlerComponent.png") **Confirmation Handler** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConfirmationHandler** component is used to handle confirming an action. (what the actions are is currently not documented)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Label` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The message of the Confirmation box |
| `Color` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The color of the button before confirming is allowed. |
| `OriginalLabel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The original label of the conformation before allowing the user to continue. |
| `OriginalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The original color of the Confirmation before allowing the user to continue. |
| `RevertTime` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The time to allow the user to click the button. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConfirmationHandler&oldid=98350](https://wiki.resonite.com/index.php?title=Component:ConfirmationHandler&oldid=98350)"

Contents