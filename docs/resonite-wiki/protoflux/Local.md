# ProtoFlux:Local

> Source: https://wiki.resonite.com/ProtoFlux:Local

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
  * [English](https://wiki.resonite.com/ProtoFlux:Local)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ALocal "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ALocal "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:Local
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:Local#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:Local)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Local&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Local&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:Local "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:Local&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:Local "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:Local "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Local&oldid=104586 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:Local&action=info "More information about this page")


Local
*
Variables
_This article or section is a stub. You can help the Resonite wiki by expanding it._
This page is missing content because it needs many more examples, since this node is quite a complex topic. TODO: Maybe explain this in reference to variables in programming? 
Local Nodes will have the default value for their data type until written to during a context. During that context, the local node will keep the value from every write and change to it. Once the context is released, the value instantly returns to the default value, discarding the data, preventing it from being seen or networked. However, if its value is written to a [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") it will persist, allowing it to be seen by everyone in the session through the network. 
The visual on this page is not a good representation of the node's appearance in game at the moment. 
The node in game has a string in the center that can be edited like a text field. This text field actually just renames the slot of the protoflux node, and will populate with the node's name when unpacked. This is useful for naming your variables, and should have no downsides. As such, never assume this node will have their slot name contain this node's type or something similar. 
## Locals as Scoped Variables
Local nodes represent a scoped, mutable value which is commonly called a variable. Unlike [ProtoFlux:Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store") and [ProtoFlux:Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"), Local is scoped to an individual impulse context. This is similar to a variable that is defined inside of a function in an imperative programming language like [JavaScript's var keyword](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var#hoisting), etc. Upon entering the value is initialized, and it is discarded once it goes out of scope. Like with variables in functions, every ProtoFlux _impulse context_ also has its own independent (not shared) variable. 
Unlike most programming languages, a local can be referenced from outside of a context (which would be like accessing a variable from outside the function it it declared). However, outside of any context, the local will just be whatever the default value of the type is. This is a common confusion in ProtoFlux: just because you can pull a wire from a local node doesn't mean that there is anything actually there. If you need to read/write to a variable outside of contexts, use a global and persistent variable like [ProtoFlux:Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store") or [ProtoFlux:Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"). 
## See Also
  * [Contexts](https://wiki.resonite.com/Impulses#Contexts "Impulses")
  * [ProtoFlux:Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store") for the globally accessible version of this node
  * [ProtoFlux:Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") for the network synchronized version of this node


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:Local&oldid=104586](https://wiki.resonite.com/index.php?title=ProtoFlux:Local&oldid=104586)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:Local#top "Back to top \[home\]")
Contents
  * [ 1 Locals as Scoped Variables ](https://wiki.resonite.com/ProtoFlux:Local#Locals_as_Scoped_Variables)
  * [ 2 See Also ](https://wiki.resonite.com/ProtoFlux:Local#See_Also)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [Stubs](https://wiki.resonite.com/Category:Stubs "Category:Stubs")
  * [ProtoFlux:Variables](https://wiki.resonite.com/Category:ProtoFlux:Variables "Category:ProtoFlux:Variables")
  * [IVariable nodes](https://wiki.resonite.com/Category:IVariable_nodes "Category:IVariable nodes")


Last modified
This page was last edited on 16 June 2025, at 15:11.
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


