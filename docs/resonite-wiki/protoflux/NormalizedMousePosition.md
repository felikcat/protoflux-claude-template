# ProtoFlux:NormalizedMousePosition

> Source: https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition

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
  * [English](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ANormalizedMousePosition "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ANormalizedMousePosition "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:NormalizedMousePosition
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NormalizedMousePosition&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NormalizedMousePosition&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:NormalizedMousePosition&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:NormalizedMousePosition "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:NormalizedMousePosition "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NormalizedMousePosition&oldid=113137 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NormalizedMousePosition&action=info "More information about this page")


Normalized Mouse Position
*
Mouse
The `Normalized Mouse Position` node returns the local [user's](https://wiki.resonite.com/User "User") normalized mouse position from their [Resonite](https://wiki.resonite.com/Resonite "Resonite") application (0 to 1 on both the x and y axis). The normalized mouse position calculation starts at the top-left of the Resonite window. If you are focused on the Resonite window, the mouse will always be centered in that window while you move the mouse around (unless interacting with a UI or in freecam mode), giving a consistent result from this node (in this case, it is usually around 0.5 for both the X and Y axis). When the Resonite application is not focused, the cursor won't be tracked at all and will snap to the bottom left (returning "[0; 1]"). Having multiple monitors will not affect this node. 
## Outputs
### * ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
The normalized position of the mouse on the Resonite application currently. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:NormalizedMousePosition&oldid=113137](https://wiki.resonite.com/index.php?title=ProtoFlux:NormalizedMousePosition&oldid=113137)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition#top "Back to top \[home\]")
Contents
  * [ 1 Outputs ](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition#Outputs)
    * [ 1.1 * (float2) ](https://wiki.resonite.com/ProtoFlux:NormalizedMousePosition#*_\(float2\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Devices:Mouse](https://wiki.resonite.com/Category:ProtoFlux:Devices:Mouse "Category:ProtoFlux:Devices:Mouse")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 19 September 2025, at 21:07.
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


