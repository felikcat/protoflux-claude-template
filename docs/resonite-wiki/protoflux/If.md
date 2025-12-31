# ProtoFlux:If

> Source: https://wiki.resonite.com/ProtoFlux:If

If

\*

OnTrue

Condition

OnFalse

Flow

The **If** node checks and evaluates the Condition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) only when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called. After the call and evaluation, it will send a pulse out of OnTrue ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) if Condition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) is `true` or OnFalse ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) if it is `false`.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want something similar to this but with data, [values](https://wiki.resonite.com/Value_Type "Value Type"), or [references](https://wiki.resonite.com/Reference_Type "Reference Type"), use the [Conditional](https://wiki.resonite.com/ProtoFlux:Conditional "ProtoFlux:Conditional") node instead.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Triggers this node to check Condition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) and send an impulse down OnTrue ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) or OnFalse ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) respectively.

### Condition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

A boolean to check only when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed.

## Outputs

### OnTrue ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and Condition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) is true.

### OnFalse ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and Condition ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) is false.

## Examples

- [an if node being used to filter the flow of an impulse chain.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_if_node.webp "File:Protoflux example if node.webp")

an if node being used to filter the flow of an impulse chain.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:If&oldid=87494](https://wiki.resonite.com/index.php?title=ProtoFlux:If&oldid=87494)"

Contents