# Creational Design Pattern

## Context and Problem Statement

I need to decide on a design pattern to provide a standardised, flexible mechanism for instatiating complex objects.

## Considered Options

- No design pattern
- Factory Pattern
- Builder Pattern

## Decision Outcome

Chosen option: "Builder Pattern", because:

- Design patterns act as building blocks for building complex software, reduce system complexity and can raise the level at which one programs (Gamma et al., 1993). Not using any if there is an applicable pattern would therefore be a disadvantage.
- The algorithm for creating complex objects (visa application and visa) should be independent of the parts which make them up.
- The construction process must allow for different representations of the object being constructed (Gamma et al., 1994). For example, the applications will have different types of documentation and additional information required.

## Consequences

Positive

- There will be a standardised way of handling complex object creation.
- Handling different types of visa and applications for different visa types will be simpler.
- New types of visa with different required documentation and additional information may be added to the system without much hassle.

Negative

- This pattern will increase the amount of code used for the solution.

## Status

Accepted on 1/12/2023

Revised on 8/12/2023

Updated Decision - Chosen option "No design pattern"

After reviewing the data design and C4 level 4 diagram, it was decided that the visa application objects where not complex enough to require a design pattern dedicated to handling their creation, and that adding one would only increase the complexity of the application.
