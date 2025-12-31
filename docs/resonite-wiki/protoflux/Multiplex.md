# ProtoFlux:Multiplex

> Source: https://wiki.resonite.com/ProtoFlux:Multiplex

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
  * [English](https://wiki.resonite.com/ProtoFlux:Multiplex)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AMultiplex "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AMultiplex "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:Multiplex
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:Multiplex#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:Multiplex)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Multiplex&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Multiplex&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:Multiplex "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:Multiplex&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:Multiplex "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:Multiplex "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Multiplex&oldid=103975 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Multiplex&action=info "More information about this page")


Multiplex
Index
Output
Inputs
InputCount
+
-
Utility
The `Multiplex` node is a node that changes its output to a specific input based on its index. 
The node can be used as a fixed-size* array in [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") or to iterate over multiple [values](https://wiki.resonite.com/Value_Type "Value Type") or variables in a [For Loop](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For"). The size of a multiplex can be near infinite, and can multiplex any [Type](https://wiki.resonite.com/Type:Type "Type:Type"). 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
If you are looking to switch between only 2 values or objects, consider using a [Conditional](https://wiki.resonite.com/ProtoFlux:Conditional "ProtoFlux:Conditional") instead. 
## Inputs
### Index ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
Selects the input value for the output. 
### Inputs (Generic)
A fixed-size* array of items with a type that will always match Output's type. 
## Outputs
### Output (Generic)
Returns the selected value from the selected index. 
### InputCount ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The number of inputs in the fixed-size* array of items in Inputs. 
  

## Examples
  * [Example of how to use a Multiplex with a For Loop to show how it can be used to make code simpler.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Multiplex.webp "File:Protoflux example Multiplex.webp")
Example of how to use a Multiplex with a [For Loop](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") to show how it can be used to make code simpler.


  

## Footnotes
* It can be made bigger or smaller while editing the flux. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:Multiplex&oldid=103975](https://wiki.resonite.com/index.php?title=ProtoFlux:Multiplex&oldid=103975)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:Multiplex#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:Multiplex#Inputs)
    * [ 1.1 Index (int) ](https://wiki.resonite.com/ProtoFlux:Multiplex#Index_\(int\))
    * [ 1.2 Inputs (Generic) ](https://wiki.resonite.com/ProtoFlux:Multiplex#Inputs_\(Generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:Multiplex#Outputs)
    * [ 2.1 Output (Generic) ](https://wiki.resonite.com/ProtoFlux:Multiplex#Output_\(Generic\))
    * [ 2.2 InputCount (int) ](https://wiki.resonite.com/ProtoFlux:Multiplex#InputCount_\(int\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:Multiplex#Examples)
  * [ 4 Footnotes ](https://wiki.resonite.com/ProtoFlux:Multiplex#Footnotes)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Utility](https://wiki.resonite.com/Category:ProtoFlux:Utility "Category:ProtoFlux:Utility")


Last modified
This page was last edited on 8 June 2025, at 12:48.
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


