<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Introduction.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Introduction

ProtoGraph is a declarative language that compiles to ProtoFlux. It helps you build high quality and maintainable software by complementing ProtoFlux. It focuses on simple language constructs that make it easy to build a mental model of what the generated ProtoFlux will look like and strong tool integration to make testing and deploying in Resonite fast and convenient.

This language reference is designed as a guide to teach:

- The basics of writing ProtoGraph
- How to use ProtoGraph as a tool for building things in Resonite
- Programming principles and patterns to help write better software

## Ecosystem Goals

ProtoGraph and its related ecosystem are tools for making it easier to write better software in Resonite. This includes the goals:

- Basic and explicit syntax that is easy to mentally translate between ProtoFlux and ProtoGraph
- Accessible to people that haven't programmed (traditionally) before and have only seen ProtoFlux
- Easy to read, write, and refactor modular code for programmers building complex projects in Resonite
- Helps you to write valid code: if your program compiles without errors or warnings then you should have a valid program where all wires are connected without issues
- Target supported Resonite formats for future compatibility

## Name and Logo Etymology

- **Prot-** : "first"
- **Graph**: "write" (Greek)
- **Flu-** : "flow" (Latin)

So _ProtoGraph_ means "first writing" in comparison to _ProtoFlux_ which means "first flow". Like in the ProtoFlux logo, the last letter in ProtoGraph is surrounded by colored "( )" but in a retalic font (lean back instead of forward). The coloration is complementary to ProtoFlux: purple/blue & yellow/orange. The "h" in ProtoGraph is stylized as a "λ" (the lowercase Greek letter lambda) as a reference to the functional influences of ProtoGraph.

## Influences

Like any programming language, ProtoGraph is influenced by many others including:

- **F#**: Functional .NET for writing succinct, robust, and performant code. Syntax is heavily drawn from the F# style and the wider .NET ecosystem that Resonite uses.

- **Elm**: A delightful language for reliable web apps. A focus on simplicity, correctness, and a lovable compiler. If it compiles, it usually works, and if it doesn't then the compiler tells you why and how to fix it.

- **Odin**: C for the modern computer for sane and joyful software development. Chose clear over clever, make it easy to do it correctly by default, and make the structure of the runtime transparent to the user.
