# ProtoFlux:GetUserGrabber

> Source: https://wiki.resonite.com/ProtoFlux:GetUserGrabber

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
  * [English](https://wiki.resonite.com/ProtoFlux:GetUserGrabber)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGetUserGrabber "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGetUserGrabber "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GetUserGrabber
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GetUserGrabber)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetUserGrabber&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetUserGrabber&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GetUserGrabber "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GetUserGrabber&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GetUserGrabber "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GetUserGrabber "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetUserGrabber&oldid=109927 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetUserGrabber&action=info "More information about this page")


Get User Grabber
User
*
Node
Grabbable
Get User Grabber is a ProtoFlux node that allows for getting the grabber sphere a user has on a specific [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). will use local user and left hand by default. This node will only give an output for `LeftHand` or `RightHand` [BodyNodes](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"). 
[989onan](https://wiki.resonite.com/User:989onan "User:989onan") Hot Take: This node using [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") rather than [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality") is probably because [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") was thinking of adding future support for devices that can allow you to grab things with your Jaw or feet. Although there seems to be no plans for this anywhere. 
## Inputs
### User ([User](https://wiki.resonite.com/Type:User "Type:User"))
The user to get a [Grabber](https://wiki.resonite.com/Type:Grabber "Type:Grabber") for. 
### Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))
The body node on the provided User ([User](https://wiki.resonite.com/Type:User "Type:User")) to find a [Grabber](https://wiki.resonite.com/Type:Grabber "Type:Grabber") on. 
Examples: `LeftHand` or `RightHand`
## Outputs
### * ([Grabber](https://wiki.resonite.com/Type:Grabber "Type:Grabber"))
The user's [Grabber](https://wiki.resonite.com/Type:Grabber "Type:Grabber") on the provided [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") (`LeftHand` or `RightHand`) 
## Examples
  * [An example of Get User Grabber being used in some ProtoFlux code.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Get_User_Grabber.webp "File:Protoflux example Get User Grabber.webp")
An example of Get User Grabber being used in some ProtoFlux code.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GetUserGrabber&oldid=109927](https://wiki.resonite.com/index.php?title=ProtoFlux:GetUserGrabber&oldid=109927)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#Inputs)
    * [ 1.1 User (User) ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#User_\(User\))
    * [ 1.2 Node (BodyNode) ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#Node_\(BodyNode\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#Outputs)
    * [ 2.1 * (Grabber) ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#*_\(Grabber\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:GetUserGrabber#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Interaction:Grabbable](https://wiki.resonite.com/Category:ProtoFlux:Interaction:Grabbable "Category:ProtoFlux:Interaction:Grabbable")


Last modified
This page was last edited on 21 August 2025, at 00:21.
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


