# ProtoFlux:FireWhileTrue

> Source: https://wiki.resonite.com/ProtoFlux:FireWhileTrue

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
  * [English](https://wiki.resonite.com/ProtoFlux:FireWhileTrue)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFireWhileTrue "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFireWhileTrue "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FireWhileTrue
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FireWhileTrue)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireWhileTrue&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireWhileTrue&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FireWhileTrue "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FireWhileTrue&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FireWhileTrue "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FireWhileTrue "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireWhileTrue&oldid=109799 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireWhileTrue&action=info "More information about this page")


Fire While True
Condition
OnUpdate
UpdatingUser
null
∅
SkipIfNull
null
∅
Flow
  

## Usage
You can use this node for constantly firing a gun, or something where a drive cannot be used and you need to create events every game tick while a value is true. 
## Inputs
### Condition ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
The value that needs to be true for this node to start sending impluses out of OnUpdate. 
By default it will be null, which will allow impulses even if UpdatingUser is null. 
## Outputs
### OnUpdate ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Will send impulses at the game tick rate of the user in UpdatingUser only while UpdatingUser sees Condition as true. 
## Globals
### UpdatingUser ([User](https://wiki.resonite.com/Type:User "Type:User")):
The User who will monitor the input Condition boolean and will handle sending the impulses. If they don't see the value as true it won't fire, even if someone else does see it true. 
### SkipIfNull ([Nullable<bool>](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1"))
The value that controls whether or not impulses from the output are sent if the UpdatingUser input is null. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FireWhileTrue&oldid=109799](https://wiki.resonite.com/index.php?title=ProtoFlux:FireWhileTrue&oldid=109799)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#top "Back to top \[home\]")
Contents
  * [ 1 Usage ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#Usage)
  * [ 2 Inputs ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#Inputs)
    * [ 2.1 Condition (bool) ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#Condition_\(bool\))
  * [ 3 Outputs ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#Outputs)
    * [ 3.1 OnUpdate (Call) ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#OnUpdate_\(Call\))
  * [ 4 Globals ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#Globals)
    * [ 4.1 UpdatingUser (User): ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#UpdatingUser_\(User\):)
    * [ 4.2 SkipIfNull (Nullable<bool>) ](https://wiki.resonite.com/ProtoFlux:FireWhileTrue#SkipIfNull_\(Nullable<bool>\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow "Category:ProtoFlux:Flow")


Last modified
This page was last edited on 21 August 2025, at 00:15.
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


