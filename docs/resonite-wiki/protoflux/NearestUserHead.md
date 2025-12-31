# ProtoFlux:NearestUserHead

> Source: https://wiki.resonite.com/ProtoFlux:NearestUserHead

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
  * [English](https://wiki.resonite.com/ProtoFlux:NearestUserHead)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ANearestUserHead "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ANearestUserHead "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:NearestUserHead
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:NearestUserHead#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:NearestUserHead)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NearestUserHead&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NearestUserHead&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:NearestUserHead "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:NearestUserHead&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:NearestUserHead "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:NearestUserHead "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NearestUserHead&oldid=110307 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:NearestUserHead&action=info "More information about this page")


Nearest User Head
Reference
Slot
IgnoreUser
User
IgnoreAFK
Distance
Avatars
Nearest User Head is a protoflux node that returns the closest user head to a slot and the head's user, or closest to the root if not provided a slot. This will also ignore the user provided to IgnoreUser ([User](https://wiki.resonite.com/Type:User "Type:User")). 
## Inputs
## Outputs
### Reference ([Slot](https://wiki.resonite.com/Slot "Slot"))
The slot which to use as a point to find the closest head to. 
### IgnoreUser ([User](https://wiki.resonite.com/Type:User "Type:User"))
The user to ignore when looking for the nearest head. 
### IgnoreAFK ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Will not return a head position from a user that is not currently focused into the world. 
### Slot
The slot of the head when found. 
### User ([User](https://wiki.resonite.com/Type:User "Type:User"))
The user of the head that was found. 
### Distance ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
How far away the found head was. 
  

## Examples
  * [And example of Nearest User Head being used in relation to controlling who should simulate an item when the host is afk.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Nearest_User_Head.webp "File:Protoflux example Nearest User Head.webp")
And example of Nearest User Head being used in relation to controlling who should simulate an item when the host is afk.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:NearestUserHead&oldid=110307](https://wiki.resonite.com/index.php?title=ProtoFlux:NearestUserHead&oldid=110307)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#Inputs)
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#Outputs)
    * [ 2.1 Reference (Slot) ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#Reference_\(Slot\))
    * [ 2.2 IgnoreUser (User) ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#IgnoreUser_\(User\))
    * [ 2.3 IgnoreAFK (bool) ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#IgnoreAFK_\(bool\))
    * [ 2.4 Slot ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#Slot)
    * [ 2.5 User (User) ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#User_\(User\))
    * [ 2.6 Distance (float) ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#Distance_\(float\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:NearestUserHead#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Avatars](https://wiki.resonite.com/Category:ProtoFlux:Avatars "Category:ProtoFlux:Avatars")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 21 August 2025, at 00:27.
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


