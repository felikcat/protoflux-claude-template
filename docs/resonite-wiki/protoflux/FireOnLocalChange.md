# ProtoFlux:FireOnLocalChange

> Source: https://wiki.resonite.com/ProtoFlux:FireOnLocalChange

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
  * [English](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFireOnLocalChange "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFireOnLocalChange "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FireOnLocalChange
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnLocalChange&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnLocalChange&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FireOnLocalChange&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FireOnLocalChange "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FireOnLocalChange "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnLocalChange&oldid=113127 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnLocalChange&action=info "More information about this page")


FireOnLocalChange
Value
OnChange
Flow
The **FireOnLocalChange** node will [listen](https://wiki.resonite.com/Type:IExecutionChangeListener%601 "Type:IExecutionChangeListener`1") for changes on its input and fire an [impulse](https://wiki.resonite.com/Impulse "Impulse") whenever the client detects a change in value across [updates](https://wiki.resonite.com/Update "Update"). 
Unlike [its non-local equivalent](https://wiki.resonite.com/ProtoFlux:FireOnChange "ProtoFlux:FireOnChange"), every user's client will be listening for changes and fire impulses owned by themselves as opposed to only one user. This is useful when a time-sensitive value is already evaluated locally, making this node work without extra network delay. 
## Inputs
### Value (Generic)
The value or object that should be listened to for changes. 
## Outputs
### OnChange ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Fires a single [impulse](https://wiki.resonite.com/Impulse "Impulse") owned by the local user whenever the provided input changes value across updates. 
## See also
  * [ProtoFlux:FireOnChange](https://wiki.resonite.com/ProtoFlux:FireOnChange "ProtoFlux:FireOnChange") for the non-local equivalent of this node where a user to fire the impulse on can be specified.
  * [ProtoFlux:FireOnLocalTrue](https://wiki.resonite.com/ProtoFlux:FireOnLocalTrue "ProtoFlux:FireOnLocalTrue")
  * [ProtoFlux:FireOnLocalFalse](https://wiki.resonite.com/ProtoFlux:FireOnLocalFalse "ProtoFlux:FireOnLocalFalse")


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnLocalChange&oldid=113127](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnLocalChange&oldid=113127)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#Inputs)
    * [ 1.1 Value (Generic) ](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#Value_\(Generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#Outputs)
    * [ 2.1 OnChange (Call) ](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#OnChange_\(Call\))
  * [ 3 See also ](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange#See_also)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow "Category:ProtoFlux:Flow")
  * [Listener nodes](https://wiki.resonite.com/Category:Listener_nodes "Category:Listener nodes")


Last modified
This page was last edited on 19 September 2025, at 08:50.
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


