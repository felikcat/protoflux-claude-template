# ProtoFlux:LocalLeakyImpulseBucket

> Source: https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket

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
  * [English](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ALocalLeakyImpulseBucket "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ALocalLeakyImpulseBucket "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:LocalLeakyImpulseBucket
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalLeakyImpulseBucket&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalLeakyImpulseBucket&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:LocalLeakyImpulseBucket&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:LocalLeakyImpulseBucket "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:LocalLeakyImpulseBucket "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalLeakyImpulseBucket&oldid=110225 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalLeakyImpulseBucket&action=info "More information about this page")


Local Leaky Impulse Bucket
Trigger
Pulse
Reset
Overflow
Interval
CurrentCapacity
MaximumCapacity
Flow
Local Leaky Impulse Bucket is a ProtoFlux node that will count how many impulses have been sent to it through Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses")), and if the capacity goes over MaximumCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) it will send an impulse. The CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) is local for every user. 
Note: There is currently a bug with this node where it will send impulses out of Overflow ([Continuation](https://wiki.resonite.com/Impulses "Impulses")) regardless of it's capacity when it should be when it overflows past the number specified in MaximumCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) [issue 145](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/145). 
## Inputs
### Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Add one to CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) and send an impulse out of Pulse ([Call](https://wiki.resonite.com/Impulses "Impulses")). 
### Reset ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Will reset CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) for the local user. 
### Interval ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
How many seconds that the node will keep impulses for before one """leaks out the bottom of the bucket""", decreasing CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) by one for the local user. 
### MaximumCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The maximum amount of Impulses that this node can store locally till the next impulse would go out of Overflow ([Continuation](https://wiki.resonite.com/Impulses "Impulses")) instead of Pulse ([Call](https://wiki.resonite.com/Impulses "Impulses"))***. 
***: See note above. 
## Outputs
### CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
Will increase by one every time Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed. it will decrease by one every Interval ([float](https://wiki.resonite.com/Type:Float "Type:Float")) seconds. It will also reset to 0 when Reset ([Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed. 
### Overflow ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
this will send an impulse when MaximumCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) is equal to CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) locally and Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed***. 
***: See note above. 
### Pulse ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Fires every time Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed unless MaximumCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) is equal to CurrentCapacity ([int](https://wiki.resonite.com/Type:Int "Type:Int")) locally then it will go out of Overflow ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))***. 
***: See note above. 
## Examples
  * [Local leaky Impulse Bucket being used on a button that plays an alternative audio clip only if it is pressed many times very quickly in a row.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=PrptpFlux_example_Local_Leaky_Impulse_Bucket.png "File:PrptpFlux example Local Leaky Impulse Bucket.png")
Local leaky Impulse Bucket being used on a button that plays an alternative audio clip only if it is pressed many times very quickly in a row.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:LocalLeakyImpulseBucket&oldid=110225](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalLeakyImpulseBucket&oldid=110225)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Inputs)
    * [ 1.1 Trigger (Call) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Trigger_\(Call\))
    * [ 1.2 Reset (Call) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Reset_\(Call\))
    * [ 1.3 Interval (float) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Interval_\(float\))
    * [ 1.4 MaximumCapacity (int) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#MaximumCapacity_\(int\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Outputs)
    * [ 2.1 CurrentCapacity (int) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#CurrentCapacity_\(int\))
    * [ 2.2 Overflow (Continuation) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Overflow_\(Continuation\))
    * [ 2.3 Pulse (Call) ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Pulse_\(Call\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:LocalLeakyImpulseBucket#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow "Category:ProtoFlux:Flow")


Last modified
This page was last edited on 21 August 2025, at 00:26.
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


