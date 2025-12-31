# ProtoFlux:NotifyModified

> Source: https://wiki.resonite.com/ProtoFlux:NotifyModified

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
  * [English](https://wiki.resonite.com/ProtoFlux:NotifyModified)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ANotifyModified "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ANotifyModified "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:NotifyModified
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:NotifyModified#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:NotifyModified)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NotifyModified&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NotifyModified&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:NotifyModified "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:NotifyModified&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:NotifyModified "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:NotifyModified "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NotifyModified&oldid=110323 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NotifyModified&action=info "More information about this page")


Notify Modified
*
Next
ModifiedComponent
Utility
The `Notify Modified` node takes in an [IComponent](https://wiki.resonite.com/Type:IComponent "Type:IComponent"), and when called will invoke the `NotifyModified` method on the input [Component](https://wiki.resonite.com/Component "Component"). Used for components which implement [IModifiedEventReceiver](https://wiki.resonite.com/index.php?title=Type:IModifiedEventReceiver&action=edit&redlink=1 "Type:IModifiedEventReceiver \(page does not exist\)") like [GridContainerPreset](https://wiki.resonite.com/Component:GridContainerPreset "Component:GridContainerPreset") and [Workspace](https://wiki.resonite.com/Component:Workspace "Component:Workspace"). 
## Inputs
### * ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Calls an impulse to check if a component was modified. 
### ModifiedComponent ([IComponent](https://wiki.resonite.com/Type:IComponent "Type:IComponent"))
The component to check. 
## Outputs
### Next ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Continue the code from here. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:NotifyModified&oldid=110323](https://wiki.resonite.com/index.php?title=ProtoFlux:NotifyModified&oldid=110323)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:NotifyModified#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:NotifyModified#Inputs)
    * [ 1.1 * (Call) ](https://wiki.resonite.com/ProtoFlux:NotifyModified#*_\(Call\))
    * [ 1.2 ModifiedComponent (IComponent) ](https://wiki.resonite.com/ProtoFlux:NotifyModified#ModifiedComponent_\(IComponent\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:NotifyModified#Outputs)
    * [ 2.1 Next (Continuation) ](https://wiki.resonite.com/ProtoFlux:NotifyModified#Next_\(Continuation\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Utility](https://wiki.resonite.com/Category:ProtoFlux:Utility "Category:ProtoFlux:Utility")


Last modified
This page was last edited on 21 August 2025, at 00:28.
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


