# ProtoFlux:Store

> Source: https://wiki.resonite.com/ProtoFlux:Store

Store

\*

Variables

_This article or section is a stub. You can help the Resonite wiki by expanding it._

This page is missing content because it needs many more examples, since this node is quite a complex topic. TODO: Maybe explain this in reference to variables in programming?

A Store is a variable that is not networked and not part of the data model. Each user can have a unique value for themselves inside of a Store and it is not specific to any context, which means it can be used across many objects and ProtoFlux scripts or even as part of a drive. This is similar to what happens when you use a [ValueUserOverride](https://wiki.resonite.com/Component:ValueUserOverride "Component:ValueUserOverride") on a field, however it does behave slightly differently: It will not update its value automatically when written to from other sources, and you will usually need to use a [Continuous Relay](https://wiki.resonite.com/ProtoFlux:Continuously_Changing_Relay "ProtoFlux:Continuously Changing Relay") with Stores to make them update in the same way that a data model field would.

The visual on this page is not a good representation of the node's appearance in game at the moment.

The node in game has a string in the center that can be edited like a text field. This text field actually just renames the slot of the protoflux node, and will populate with the node's name when unpacked. This is useful for naming your variables, and should have no downsides. As such, never assume this node will have their slot name contain this node's type or something similar.

## Stores as Global Variables

A store node is a global, mutable reference to a value which is commonly called a variable in programming (internally, the StoredValue/Object node class implements the IVariable interface). Being global means that there is only one variable that exists for the entire lifetime of the program that is represented by this node, and it is accessible from all other parts of the program. In other programming languages this would be achieved with things like the global keyword in Python or static classes in C#.

In most structured programming, the use of global variables is considered bad design because managing global mutable state adds a lot of complexity and makes it easy to introduce strange bugs. If possible, consider refactoring your algorithms to use immutable values (such as [ProtoFlux:Input](https://wiki.resonite.com/ProtoFlux:Input "ProtoFlux:Input")) or use scoped variables like [ProtoFlux:Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local").

## Reading

The store can be read similar to other data outputs because it is data, but be aware of the need to use a [Continuous Relay](https://wiki.resonite.com/ProtoFlux:Continuously_Changing_Relay "ProtoFlux:Continuously Changing Relay") if you want to watch the value to detect changes. Otherwise its value will only be queried when one of the downstream nodes pulls for it (for example an impulse). TODO: validate

TODO: example reading with relay

TODO: example reading without relay

## Writing

Writing to the store can be accomplished with the [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") node.

TODO: example with write node

## Scoping

A Store is scoped to the user. This is broader than the [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local") but narrower than the [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store"). Compared to other programming languages, it is most similar to a global variable.

TODO: example of referencing a store from different locations

## See Also

- [Contexts](https://wiki.resonite.com/Impulses#Contexts "Impulses")
- [ProtoFlux:Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") for the network synchronized version of this node
- [ProtoFlux:Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local") for the locally scoped version of this node

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Store&oldid=104577](https://wiki.resonite.com/index.php?title=ProtoFlux:Store&oldid=104577)"

Contents