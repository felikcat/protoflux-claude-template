# ProtoFlux:For

> Source: https://wiki.resonite.com/ProtoFlux:For

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
  * [English](https://wiki.resonite.com/ProtoFlux:For)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFor "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFor "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:For
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:For#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:For)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:For&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:For&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:For "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:For&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:For "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:For "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:For&oldid=93263 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:For&action=info "More information about this page")


For
*
LoopStart
Count
LoopIteration
Reverse
LoopEnd
iteration
Flow
The **For** node is used to perform looping operations by allowing one to fire impulses a set amount of times. 
## Inputs
### * ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Begin the for loop. 
### Count ([Int](https://wiki.resonite.com/Type:Int "Type:Int"))
The amount of times to trigger `LoopIteration`. Will not trigger any iterations if less than 1. 
### Reverse ([Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
If `True`, the `Iteration` output will start at `Count - 1` and go down towards `0`. 
## Outputs
### LoopStart ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Fires after `*` is pulsed and before any iterations are done. Will be pulsed even if `Count < 1`. 
### LoopIteration ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Fires for each iteration of the loop. This impulse is triggered <count>Count amount of times and the next iteration will only be fired once the current iteration's [context](https://wiki.resonite.com/Context "Context") is finished. 
### LoopEnd ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires after the final `LoopIteration` completes execution. 
### Iteration ([Int](https://wiki.resonite.com/Type:Int "Type:Int"))
For each `LoopIteration`, this output is set to be the index of the iteration for said iteration's context. By default, this will start at `0` and increment until `Count - 1` unless `Reverse` is `True`. 
## Examples
  * [![Using the for node to iteratively check if a child slot has the tag 'foo'. and replace it with 'bar' using the Children Count and Get Child nodes.](https://wiki.resonite.com/images/thumb/4/40/For_node_example.png/480px-For_node_example.png)](https://wiki.resonite.com/File:For_node_example.png "Using the for node to iteratively check if a child slot has the tag 'foo'. and replace it with 'bar' using the Children Count and Get Child nodes.")
Using the **for** node to iteratively check if a child slot has the tag 'foo'. and replace it with 'bar' using the [Children Count](https://wiki.resonite.com/Children_Count_\(ProtoFlux\) "Children Count \(ProtoFlux\)") and [Get Child](https://wiki.resonite.com/Get_Child_\(ProtoFlux\) "Get Child \(ProtoFlux\)") nodes.


## See Also
  * [ProtoFlux:Async For](https://wiki.resonite.com/ProtoFlux:Async_For "ProtoFlux:Async For") for the [async](https://wiki.resonite.com/Async "Async") variant of this node.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:For&oldid=93263](https://wiki.resonite.com/index.php?title=ProtoFlux:For&oldid=93263)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:For#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:For#Inputs)
    * [ 1.1 * (Call) ](https://wiki.resonite.com/ProtoFlux:For#*_\(Call\))
    * [ 1.2 Count (Int) ](https://wiki.resonite.com/ProtoFlux:For#Count_\(Int\))
    * [ 1.3 Reverse (Bool) ](https://wiki.resonite.com/ProtoFlux:For#Reverse_\(Bool\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:For#Outputs)
    * [ 2.1 LoopStart (Call) ](https://wiki.resonite.com/ProtoFlux:For#LoopStart_\(Call\))
    * [ 2.2 LoopIteration (Call) ](https://wiki.resonite.com/ProtoFlux:For#LoopIteration_\(Call\))
    * [ 2.3 LoopEnd (Continuation) ](https://wiki.resonite.com/ProtoFlux:For#LoopEnd_\(Continuation\))
    * [ 2.4 Iteration (Int) ](https://wiki.resonite.com/ProtoFlux:For#Iteration_\(Int\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:For#Examples)
  * [ 4 See Also ](https://wiki.resonite.com/ProtoFlux:For#See_Also)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow "Category:ProtoFlux:Flow")


Last modified
This page was last edited on 15 December 2024, at 19:11.
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


