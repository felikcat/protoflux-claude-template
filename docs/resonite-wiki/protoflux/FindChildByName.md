# ProtoFlux:FindChildByName

> Source: https://wiki.resonite.com/ProtoFlux:FindChildByName

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
  * [English](https://wiki.resonite.com/ProtoFlux:FindChildByName)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFindChildByName "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFindChildByName "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FindChildByName
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FindChildByName#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FindChildByName)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindChildByName&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindChildByName&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FindChildByName "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FindChildByName&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FindChildByName "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FindChildByName "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindChildByName&oldid=109775 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindChildByName&action=info "More information about this page")


Find Child By Name
Instance
*
Name
MatchSubstring
IgnoreCase
SearchDepth
Slots
Finds a child object under Instance ([Slot](https://wiki.resonite.com/Slot "Slot")) that matches the given arguments 
![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)
Using this node to search the entire root in ProtoFlux that tries to evaluate every frame will generate considerable frame lag. If searching the root has to be done, put the result into a cached variable ([Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store")) rather than searching every game tick. 
## Inputs
### Instance ([Slot](https://wiki.resonite.com/Slot "Slot"))
The slot to scan for children with. 
### Name ([String](https://wiki.resonite.com/Type:String "Type:String"))
The name to look for under Instance ([Slot](https://wiki.resonite.com/Slot "Slot")). 
### MatchSubstring ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Whether to search for children under Instance ([Slot](https://wiki.resonite.com/Slot "Slot")) that their name contains Name ([String](https://wiki.resonite.com/Type:String "Type:String")) instead of the entire name being equal. 
### IgnoreCase ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Whether the capitalization should matter or not when searching for a child under Instance ([Slot](https://wiki.resonite.com/Slot "Slot")). 
### SearchDepth ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
How far to search for a child with the provided search arguments 
Examples: 0 > Search immediate children. 1 > Search children of slot including those slot's children. -1 > Search infinitely far down (HEAVY) 
## Outputs
### * ([Slot](https://wiki.resonite.com/Slot "Slot"))
The result of the search. 
## Examples
  * [An example code finding slots under and above other slots in a list, one of the nodes is a Find Child By Name.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_find_by.webp "File:ProtoFlux example find by.webp")
An example code finding slots under and above other slots in a list, one of the nodes is a Find Child By Name.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FindChildByName&oldid=109775](https://wiki.resonite.com/index.php?title=ProtoFlux:FindChildByName&oldid=109775)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FindChildByName#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FindChildByName#Inputs)
    * [ 1.1 Instance (Slot) ](https://wiki.resonite.com/ProtoFlux:FindChildByName#Instance_\(Slot\))
    * [ 1.2 Name (String) ](https://wiki.resonite.com/ProtoFlux:FindChildByName#Name_\(String\))
    * [ 1.3 MatchSubstring (bool) ](https://wiki.resonite.com/ProtoFlux:FindChildByName#MatchSubstring_\(bool\))
    * [ 1.4 IgnoreCase (bool) ](https://wiki.resonite.com/ProtoFlux:FindChildByName#IgnoreCase_\(bool\))
    * [ 1.5 SearchDepth (int) ](https://wiki.resonite.com/ProtoFlux:FindChildByName#SearchDepth_\(int\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FindChildByName#Outputs)
    * [ 2.1 * (Slot) ](https://wiki.resonite.com/ProtoFlux:FindChildByName#*_\(Slot\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:FindChildByName#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Slots:Searching](https://wiki.resonite.com/Category:ProtoFlux:Slots:Searching "Category:ProtoFlux:Slots:Searching")


Last modified
This page was last edited on 20 August 2025, at 23:52.
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


