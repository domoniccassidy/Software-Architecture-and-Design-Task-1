# Architecture Style

## Context and Problem Statement

I need to decide upon an architecture style for the AFS visa processing service

## Considered Options

- Event Driven Architecture
- Service Oriented Architecture
- Layered Architecture
- Component Based Architecture

## Decision Outcome

Chosen option "Service Oriented Architecture" because:

- Helps realise high priority non-functional requirements such as scalability, reliability, and availability
- Other styles mainly realise lower priority non-functional requirements
- I have experience working with Service Oriented Architecure
- "SOA is a valuable approach when an application is expected to undergo significant change in platform requirement, load requirement, integration requirement, and scalability" (Choi, et al., 2010), which I do as the number of visa applicants fluctuates throughout the year.

## Consequences

Positive

- Provides great system scalability (Pedamkar, 2023)
- Allows for easy maintainability of the system (Pedamkar, 2023)
- Easier maintainability will have positive impacts on reliability and availability (Techspirited, n.d.)

Negative

- System will be less performant than if another style was chosen (Techspirited, n.d.)
- SOA requires a high bandwidth server (Pedamkar, 2023)

# Status

Accepted on 24/10/2023
