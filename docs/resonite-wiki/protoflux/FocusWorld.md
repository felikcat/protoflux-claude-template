# ProtoFlux:FocusWorld

> Source: https://wiki.resonite.com/ProtoFlux:FocusWorld

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
  * [English](https://wiki.resonite.com/ProtoFlux:FocusWorld)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFocusWorld "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFocusWorld "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FocusWorld
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FocusWorld#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FocusWorld)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FocusWorld&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FocusWorld&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FocusWorld "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FocusWorld&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FocusWorld "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FocusWorld "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FocusWorld&oldid=109809 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FocusWorld&action=info "More information about this page")


Focus World
*
OnNotFound
URL
OnFocused
WorldLink
CloseCurrent
World
The `Focus World` node allows a user to focus on a world by giving it a ressession link as the [Url](https://wiki.resonite.com/Type:Uri "Type:Uri"). If the world exists (as in, already opened for the user, or available as a headless) it will work as expected. If there is no world that is open already that the ressession link is referring to, it will fail. 
Headless worlds would normally have a SessionID that is consistent that you can use to make into a resession link, allowing you to open and join these worlds with ease. 
This node is also useful when making [Exit Strategies](https://wiki.resonite.com/Exit_Strategy "Exit Strategy"), as you can set it up to where if the world is valid to focus, you can close the current world, and have the node continue from here to play a particle effect, a sound, and much more. 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
If you are the [Host User](https://wiki.resonite.com/ProtoFlux:Host_User "ProtoFlux:Host User"), closing the world with this node will only work if there are NOT unsaved changes OR the world is not allowed to be saved. Unsaved changes are determined by a bool on the UndoManager. 
## Inputs
### * ([AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))
Calls from an impulse to begin focusing a world. 
### URL ([Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))
The ressession link needed to focus a world. 
### WorldLink ([IWorldLink](https://wiki.resonite.com/index.php?title=Type:IWorldLink&action=edit&redlink=1 "Type:IWorldLink \(page does not exist\)"))
The link to a world (using the [WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink") component). This can be an alternative way of focusing a world. 
### CloseCurrent ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Should this node close the current world after we focus to a different world. 
## Outputs
### OnNotFound ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires when there is no world to focus on or the world link is not valid. 
### OnFocused ([AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))
Fires when we successfully focus a world (and only fires in that current world, not the world we are focusing to). 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FocusWorld&oldid=109809](https://wiki.resonite.com/index.php?title=ProtoFlux:FocusWorld&oldid=109809)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FocusWorld#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FocusWorld#Inputs)
    * [ 1.1 * (AsyncCall) ](https://wiki.resonite.com/ProtoFlux:FocusWorld#*_\(AsyncCall\))
    * [ 1.2 URL (Uri) ](https://wiki.resonite.com/ProtoFlux:FocusWorld#URL_\(Uri\))
    * [ 1.3 WorldLink (IWorldLink) ](https://wiki.resonite.com/ProtoFlux:FocusWorld#WorldLink_\(IWorldLink\))
    * [ 1.4 CloseCurrent (bool) ](https://wiki.resonite.com/ProtoFlux:FocusWorld#CloseCurrent_\(bool\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FocusWorld#Outputs)
    * [ 2.1 OnNotFound (Continuation) ](https://wiki.resonite.com/ProtoFlux:FocusWorld#OnNotFound_\(Continuation\))
    * [ 2.2 OnFocused (AsyncCall) ](https://wiki.resonite.com/ProtoFlux:FocusWorld#OnFocused_\(AsyncCall\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:World](https://wiki.resonite.com/Category:ProtoFlux:World "Category:ProtoFlux:World")


Last modified
This page was last edited on 21 August 2025, at 00:16.
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


