# ProtoFlux:IsUserLagging

> Source: https://wiki.resonite.com/ProtoFlux:IsUserLagging

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
  * [English](https://wiki.resonite.com/ProtoFlux:IsUserLagging)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AIsUserLagging "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AIsUserLagging "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:IsUserLagging
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:IsUserLagging#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:IsUserLagging)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:IsUserLagging&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:IsUserLagging&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:IsUserLagging "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:IsUserLagging&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:IsUserLagging "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:IsUserLagging "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:IsUserLagging&oldid=113461 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:IsUserLagging&action=info "More information about this page")


Is User Lagging
User
*
Status
The **IsUserLagging** node was added during the [2025 April Fools' update](https://wiki.resonite.com/Beta_2025.4.1.438 "Beta 2025.4.1.438") to detect if a user was "Lagging". In reality, this node returns whether the last synchronization message received by the host from the specified `User` was more than 1.5 seconds ago. 
## Inputs
### User ([User](https://wiki.resonite.com/Type:User "Type:User"))
The [user](https://wiki.resonite.com/User "User") to check. 
## Outputs
### * ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Returns whether the user is "lagging", or if the last synchronization message received by the host from the user was more than 1.5 seconds ago. This output will always be `False` for the host user. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:IsUserLagging&oldid=113461](https://wiki.resonite.com/index.php?title=ProtoFlux:IsUserLagging&oldid=113461)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:IsUserLagging#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:IsUserLagging#Inputs)
    * [ 1.1 User (User) ](https://wiki.resonite.com/ProtoFlux:IsUserLagging#User_\(User\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:IsUserLagging#Outputs)
    * [ 2.1 * (bool) ](https://wiki.resonite.com/ProtoFlux:IsUserLagging#*_\(bool\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Users:Status](https://wiki.resonite.com/Category:ProtoFlux:Users:Status "Category:ProtoFlux:Users:Status")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 9 October 2025, at 17:33.
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


