# ProtoFlux:DataModelStore

> Source: https://wiki.resonite.com/ProtoFlux:DataModelStore

Data Model Store

\*

Variables

_This article or section is a stub. You can help the Resonite wiki by expanding it._

This page is missing content because it needs many more examples, since this node is quite a complex topic. TODO: Maybe explain this in reference to variables in programming?

A [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") will allow writes to it that will persist across contexts, allowing for another impulse or script to read the variable later and act on it. This is good for storing your final value after a massive calculation as a value for a smaller drive script. If a [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") is written to multiple times in a Impulse, the last value is the value that gets networked to other users. Data model stores can be read much later, and will even keep and save their value when an item is saved.

The visual on this page is not a good representation of the node's appearance in game at the moment.

The node in game has a string in the center that can be edited like a text field. This text field actually just renames the slot of the protoflux node, and will populate with the node's name when unpacked. This is useful for naming your variables, and should have no downsides. As such, never assume this node will have their slot name contain this node's type or something similar.

## Data Model Stores as Globally Synchronized Variables

A DataModelStore node is a globally synchronized, mutable reference to a value which is commonly called a variable in programming (internally, the DataModelValue/Object node class implements the IVariable interface). Being global means that there is only one variable that exists for the entire lifetime of the program that is represented by this node, and it is accessible from all other parts of the program. In other programming languages this would be achieved with things like the global keyword in Python or static classes in C#. Furthermore because the store is synchronized, when the value is updated by _any one_ user, that update will _propagate to all the other users_ in the session. This synchronization is handled automatically by the Froox engine, so reading and writing the store is _mostly_ the same as [ProtoFlux:Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store").

In most structured programming, the use of global variables is considered bad design because managing global mutable state adds a lot of complexity and makes it easy to introduce strange bugs. However, in ProtoFlux, this is considered a common design pattern because maintaining global mutable state is the goal. It is up to the programmer to properly manage access to the data model store to keep their flux maintainable.

## See Also

- [Contexts](https://wiki.resonite.com/Impulses#Contexts "Impulses")
- [ProtoFlux:Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store") for the non-network synchronized version of this node
- [ProtoFlux:Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local") for the locally scoped version of this node

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DataModelStore&oldid=109599](https://wiki.resonite.com/index.php?title=ProtoFlux:DataModelStore&oldid=109599)"

Contents