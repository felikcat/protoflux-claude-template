# ProtoFlux:FieldHook

> Source: https://wiki.resonite.com/ProtoFlux:FieldHook

[ ![](https://wiki.resonite.com/images/1/11/Resonite_Wiki-Icon.png) ](https://wiki.resonite.com/Main_Page "Visit the main page")
Toggle search
Search [ ](https://wiki.resonite.com/Special:Random "Random page")
Toggle menu
[ ![](https://wiki.resonite.com/images/1/11/Resonite_Wiki-Icon.png) ](https://wiki.resonite.com/Main_Page "Visit the main page")
Resonite Wiki
Navigation 
  * [](https://wiki.resonite.com/Special:MyLanguage/Main_Page "Visit the main page \[z\]")
  * [](https://wiki.resonite.com/Special:RecentChanges "A list of recent changes in the wiki \[r\]")
  * [](https://wiki.resonite.com/Special:Random "Load a random page \[x\]")
  * [](https://www.mediawiki.org/wiki/Special:MyLanguage/Help:Contents)
  * [Contributing to the Wiki](https://wiki.resonite.com/Special:MyLanguage/Wiki_Contributions_%26_Translations)
  * [](https://wiki.resonite.com/Special:SpecialPages "A list of all special pages \[q\]")
  * [](https://wiki.resonite.com/Special:Upload "Upload files \[u\]")


Team 
  * [Resonite Team](https://wiki.resonite.com/Special:MyLanguage/Resonite_Team)
  * [Moderation](https://wiki.resonite.com/Special:MyLanguage/Moderation)
  * [Office Hours](https://wiki.resonite.com/Special:MyLanguage/Office_Hours)
  * [Contact Us](https://wiki.resonite.com/Special:MyLanguage/Contact_Us)


Key Information 
  * [Guidelines and Rules](https://wiki.resonite.com/Special:MyLanguage/Guidelines)
  * [FAQ](https://wiki.resonite.com/Special:MyLanguage/Frequently_Asked_Questions)
  * [How to Help](https://wiki.resonite.com/Special:MyLanguage/How_to_Help)
  * [Branding Information](https://wiki.resonite.com/Special:MyLanguage/Branding)
  * [Roadmap](https://wiki.resonite.com/Special:MyLanguage/Roadmap)
  * [Get your Patreon Rewards](https://wiki.resonite.com/Special:MyLanguage/Patreon_Linking)


notifications 
Toggle personal menu
  * Not logged in


user-interface-preferences 
  * [English](https://wiki.resonite.com/ProtoFlux:FieldHook)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFieldHook "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFieldHook "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FieldHook
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FieldHook#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FieldHook)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FieldHook&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FieldHook&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FieldHook "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FieldHook&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FieldHook "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FieldHook "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FieldHook&oldid=109765 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FieldHook&action=info "More information about this page")


Field Hook
StartDrive
OnStartDrive
StopDrive
OnStopDrive
Target
OnHook
Source
IsDriving
HookedValue
Core
The **Field Hook** node takes in a target [field](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") and the source field value, then returns if this field is [driving](https://wiki.resonite.com/Drive "Drive"), as well as allowing the [user](https://wiki.resonite.com/User "User") to start and stop driving this field. This node gives the user more control to programmatically drive fields directly using ProtoFlux. This node hooks the given field, so whenever something external tries to write to it, it will receive a pulse from OnHook as well as the value it tried to write from HookedValue. 
## Inputs
### StartDrive ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Calls an impulse to start driving the target (hooking into it). 
### StopDrive ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Calls an impulse to stop driving the target (unhooking it). 
### Target ([IField`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1"))
The target field to drive. 
### Source (Generic)
The source to drive from. 
## Outputs
### OnStartDrive ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires when we started driving the target field. 
### OnStopDrive ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires when we stopped driving the target field. 
### OnHook ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Fires when something writes to the target field while it is being driven by this node. 
### IsDriving ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Returns if the target field is being driven. 
### HookedValue (Generic)
Returns the value that was written by the OnHook call. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FieldHook&oldid=109765](https://wiki.resonite.com/index.php?title=ProtoFlux:FieldHook&oldid=109765)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FieldHook#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FieldHook#Inputs)
    * [ 1.1 StartDrive (Call) ](https://wiki.resonite.com/ProtoFlux:FieldHook#StartDrive_\(Call\))
    * [ 1.2 StopDrive (Call) ](https://wiki.resonite.com/ProtoFlux:FieldHook#StopDrive_\(Call\))
    * [ 1.3 Target (IField`1) ](https://wiki.resonite.com/ProtoFlux:FieldHook#Target_\(IField`1\))
    * [ 1.4 Source (Generic) ](https://wiki.resonite.com/ProtoFlux:FieldHook#Source_\(Generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FieldHook#Outputs)
    * [ 2.1 OnStartDrive (Continuation) ](https://wiki.resonite.com/ProtoFlux:FieldHook#OnStartDrive_\(Continuation\))
    * [ 2.2 OnStopDrive (Continuation) ](https://wiki.resonite.com/ProtoFlux:FieldHook#OnStopDrive_\(Continuation\))
    * [ 2.3 OnHook (Call) ](https://wiki.resonite.com/ProtoFlux:FieldHook#OnHook_\(Call\))
    * [ 2.4 IsDriving (bool) ](https://wiki.resonite.com/ProtoFlux:FieldHook#IsDriving_\(bool\))
    * [ 2.5 HookedValue (Generic) ](https://wiki.resonite.com/ProtoFlux:FieldHook#HookedValue_\(Generic\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Core](https://wiki.resonite.com/Category:ProtoFlux:Core "Category:ProtoFlux:Core")
  * [Listener nodes](https://wiki.resonite.com/Category:Listener_nodes "Category:Listener nodes")


Last modified
This page was last edited on 20 August 2025, at 23:51.
Resonite Wiki
[Resonite Website](https://resonite.com)
[Resonite Policies](https://resonite.com/policies)
[Resonite on Steam](https://store.steampowered.com/app/2519830/Resonite/)
  * [Privacy policy](https://wiki.resonite.com/Resonite_Wiki:Privacy_policy)
  * [About Resonite Wiki](https://wiki.resonite.com/Resonite_Wiki:About)
  * [Disclaimers](https://wiki.resonite.com/Resonite_Wiki:General_disclaimer)


Content is available under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), unless otherwise specified. 
Resonite is Copyright © Yellow Dog Man Studios s.r.o. 
  * [![Powered by MediaWiki](https://wiki.resonite.com/resources/assets/poweredby_mediawiki_88x31.png)](https://www.mediawiki.org/)


