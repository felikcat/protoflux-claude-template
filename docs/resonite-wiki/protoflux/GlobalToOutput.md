# ProtoFlux:GlobalToOutput

> Source: https://wiki.resonite.com/ProtoFlux:GlobalToOutput

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
  * [English](https://wiki.resonite.com/ProtoFlux:GlobalToOutput)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGlobalToOutput "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGlobalToOutput "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GlobalToOutput
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GlobalToOutput)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GlobalToOutput&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GlobalToOutput&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GlobalToOutput "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GlobalToOutput&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GlobalToOutput "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GlobalToOutput "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GlobalToOutput&oldid=109939 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GlobalToOutput&action=info "More information about this page")


Global To Output
*
Global
null
∅
Core
The **Global To Output** node takes in a reference to a [global value](https://wiki.resonite.com/Component:GlobalValue "Component:GlobalValue") or [global reference](https://wiki.resonite.com/Component:GlobalReference "Component:GlobalReference") and returns the data contained in that component reference. 
## Outputs
### * (Generic)
The value that was stored in a global value or global reference component. 
## Globals
### Global (Generic)
The component that is referenced. 
## Examples
To make this work, you need the following things: 
  * [Write To Global](https://wiki.resonite.com/ProtoFlux:Write_To_Global "ProtoFlux:Write To Global")
  * [Global To Output](https://wiki.resonite.com/ProtoFlux:Global_To_Output "ProtoFlux:Global To Output")
  * [Global Value](https://wiki.resonite.com/Component:GlobalValue "Component:GlobalValue") or [Global Reference](https://wiki.resonite.com/Component:GlobalReference "Component:GlobalReference")


Using primary on either global areas of the nodes will automatically make a GlobalValue/GlobalReference component. These can be accessed currently through the inspector only. Once opened in the inspector, if there are any GlobalToOutput nodes that automatically made GlobalValue/GlobalReference components on them, those can be removed in favor of any components made prior (either on WriteToGlobal nodes or on other slots that has those components) 
The last step is to reference GlobalValue/GlobalReference component in the WriteToGlobal node (or from some other slot) to the field in the GlobalToOutput node. Then call the write node and notice the value change. 
![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)
Keep in mind that the GlobalToOutput node will not update automatically if you have a display out from it already, using the [Continuously Changing Relay](https://wiki.resonite.com/ProtoFlux:Continuously_Changing_Relay "ProtoFlux:Continuously Changing Relay") will update these displays as you write values to see those displays update, although not recommended. 
  * [![ProtoFlux Global Example.](https://wiki.resonite.com/images/thumb/f/f8/ProtoFluxGlobalExample.png/480px-ProtoFluxGlobalExample.png)](https://wiki.resonite.com/File:ProtoFluxGlobalExample.png "ProtoFlux Global Example.")
ProtoFlux Global Example.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GlobalToOutput&oldid=109939](https://wiki.resonite.com/index.php?title=ProtoFlux:GlobalToOutput&oldid=109939)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#top "Back to top \[home\]")
Contents
  * [ 1 Outputs ](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#Outputs)
    * [ 1.1 * (Generic) ](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#*_\(Generic\))
  * [ 2 Globals ](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#Globals)
    * [ 2.1 Global (Generic) ](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#Global_\(Generic\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:GlobalToOutput#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Core](https://wiki.resonite.com/Category:ProtoFlux:Core "Category:ProtoFlux:Core")
  * [IVariable nodes](https://wiki.resonite.com/Category:IVariable_nodes "Category:IVariable nodes")


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


