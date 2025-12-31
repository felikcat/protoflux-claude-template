# Component:TwitchChatDialog

> Source: https://wiki.resonite.com/Component:TwitchChatDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e5/TwitchChatDialogComponent.png/510px-TwitchChatDialogComponent.png)](https://wiki.resonite.com/File:TwitchChatDialogComponent.png) **Twitch Chat Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Twitch chat dialogue is a component used to control and manage a live stream of chat messages sent by users at Twitch from a specific channel on Twitch.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas this component generated for a visual twitch chat feed. |
| `_panel` | **[LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel")** | The panel this component generated for a visual twitch chat feed. |
| `MaxMessages` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum amount of messages to keep in the message feed before deleting old ones. |
| `Interface` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [TwitchInterface](https://wiki.resonite.com/Component:TwitchInterface "Component:TwitchInterface") >** | The twitch interface that is providing and receiving events to allow this component to function. |
| `_channelName` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The text field that holds the name of the channel this component is displaying chat messages for. |
| `_viewerCount` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text object displaying the amount of users watching `_channelName` |
| `_messagesRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot to put UIX text components under which are messages sent into `_channelName`'s chat. |
| `_messagesScrollRect` | **[ScrollRect](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect")** | The scroll rectangle that is controlled to make sure it stays scrolled to the bottom as chat messages appear. |
| `_highlightPanel` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The image used for when the panel is highlighted. |
| `_highlightText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text used for when the panel is highlighted. |
| `_spriteSheet` | **[DynamicSpriteFont](https://wiki.resonite.com/Component:DynamicSpriteFont "Component:DynamicSpriteFont")** | The dynamically changing sprite font for text characters like custom twitch emojis. |
| `_fontCollection` | **[FontCollection](https://wiki.resonite.com/Component:FontCollection "Component:FontCollection")** | A list of fonts used by chat messages from twitch. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``ChannelEditingStarted:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Handles when the user starts editing the target channel name. |
| ``ChannelEditingFinished:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | Handles when the user finishes editing the target channel name. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the default Twitch chat item in Resonite Essentials.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TwitchChatDialog&oldid=100746](https://wiki.resonite.com/index.php?title=Component:TwitchChatDialog&oldid=100746)"

Contents