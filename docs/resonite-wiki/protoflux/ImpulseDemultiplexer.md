# ProtoFlux:ImpulseDemultiplexer

> Source: https://wiki.resonite.com/ProtoFlux:ImpulseDemultiplexer

Impulse Demultiplexer

Operations

OnTriggered

Index

+

-

Flow

An Impulse Demultiplexer is useful for condensing down multiple lines of execution code into one line. For example, let's say that you have 10 buttons, and you want to change a text to 10 different strings, positions, and colors using those 10 buttons. Using an Impulse Demultiplexer you can put each button into Operations (List of Impulses) on the impulse demultiplexer, then use the index in 3 different [Multiplexers](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex"). Writing the multiplexer's output to the properties of the text object now allows you to reduce what would take up to 70 nodes and 60 connections down to 43 nodes and 43 connections. And also it makes it a lot less complex and easier to read.

This node could commonly be called a switch, switchboard, router, or an impulse array.

## Inputs

### Operations (List of [Impulses](https://wiki.resonite.com/Impulses "Impulses"))

List of impulses to take impulses from.

## Outputs

### OnTriggered ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when any one of Operations (List of [Impulses](https://wiki.resonite.com/Impulses "Impulses")) is called.

### Index ( [Int](https://wiki.resonite.com/Type:Int "Type:Int"))

The position of the Impulse on the list of Operations (List of [Impulses](https://wiki.resonite.com/Impulses "Impulses")) that was called starting at 0 for the first one.

Only exists during OnTriggered ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

## Examples

- [Impulse demultiplexer being used to control the flow of an impulse chain using an Index Of First Match node.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_impulse_demultiplexer.webp "File:Protoflux example impulse demultiplexer.webp")

Impulse demultiplexer being used to control the flow of an impulse chain using an [Index Of First Match](https://wiki.resonite.com/ProtoFlux:Index_Of_First_Match "ProtoFlux:Index Of First Match") node.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ImpulseDemultiplexer&oldid=110003](https://wiki.resonite.com/index.php?title=ProtoFlux:ImpulseDemultiplexer&oldid=110003)"

Contents