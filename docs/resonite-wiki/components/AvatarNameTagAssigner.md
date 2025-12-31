# Component:AvatarNameTagAssigner

> Source: https://wiki.resonite.com/Component:AvatarNameTagAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarNameTagAssigner&diff=91184) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/40/AvatarNameTagAssignerComponent.png/510px-AvatarNameTagAssignerComponent.png)](https://wiki.resonite.com/File:AvatarNameTagAssignerComponent.png) **AvatarNameTagAssigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarNameTagAssigner** component is responsible for setting the [nametag's](https://wiki.resonite.com/Nameplate "Nameplate") text, color, and the [ContactLink](https://wiki.resonite.com/Component:ContactLink "Component:ContactLink") UserId. It basically defines what a nametag is.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LabelTargets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of string fields that should be set to the user's display name when this component is under an avatar and the avatar is equipped. |
| `UserIdTargets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of string fields that should be set to the user's UUID (aka UserID) when this component is under an avatar and the avatar is equipped. |
| `ColorTargets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | A list of colorX fields that should be set to the user's special color when this component is under an avatar and the avatar is equipped. Supporters, Staff, Mentors, and Moderators are some of the many users that get custom name plate colors through this component. |
| `OutlineTargets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | Similar to `ColorTargets` but for the outline. |
| `BackgroundTargets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | Similar to `ColorTargets` but for the background color. |
| `DequippedLabel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What text should display when the avatar this component belongs to is dequipped. You can be creative with this! |

Fields
Collapse

## Behavior

When an avatar is dequipped the DequippedLabel contents will be written to the LabelTargets, by default the DequippedLabel is "---".

## Examples

By default a user's [Name Badge](https://wiki.resonite.com/Nameplate "Nameplate") will contain a **AvatarNameTagAssigner** connected to [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer"), [TextUnlitMaterial](https://wiki.resonite.com/Component:TextUnlitMaterial "Component:TextUnlitMaterial"), and a [ContactLink](https://wiki.resonite.com/Component:ContactLink "Component:ContactLink"). The user's username will be written to the TextRenderer, their default Name Badge colors will be written to the TextUnlitMaterial, and their UserId will be written to the ContactLink.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Not unassigning these fields located in this component will result in your hard work being overwritten when equipping the avatar. Please make sure that the parts that you want overridden is referenced here, else leave those parts blank to have them customized.


## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarNameTagAssigner&oldid=91184](https://wiki.resonite.com/index.php?title=Component:AvatarNameTagAssigner&oldid=91184)"

Contents