# Data Store Architectural Patterns

## Context and Problem Statement

I must decide on which architectural patterns to implement in regards to working with a data store.

## Considered Options

- No architectural patterns
- CQRS (Command Query Responsibilty Segregation)
- Event Sourcing

## Decision Outcome

Chosen option: "CQRS and Event Sourcing", because:

- The AFS system will provide a task-based user interface and will contain complex domain models, which CQRS is appropriate for (Microsoft, n.d. -a).
- Event Sourcing is needed to capture changes to application status (e.g., "In Review" to "Requires Additional Information")
- Event Sourcing and CQRS are often used together (Microsoft, n.d. -a).

## Consequences

Positive

- Read and write workloads can be scaled independently (Microsoft, n.d. -a)
- Schemas can be optimised for reads and writes/updates respectively (Microsoft, n.d. -a)
- An audit trail will be provided to monitor all actions against an application
- These architectural patterns are widely understood and documented, helping with development and debugging

Negative

- The system must be built to handle new events regarding a change to an entity being added during the delay between adding the original event being added, the event being published, and the consumer handling it (Microsoft, n.d. -b)
- The system must ensure the write and read models are synchronised
- The application may become more complex as a result of implementing CQRS and Event Sourcing

## Status

Accepted on 22/11/2023

Revised on 30/11/2023

Updated Decision - Chosen option "No architectural patterns"

After more careful consideration, it was decided that the complexity of CQRS and Event Sourcing were too high for the benefits. On further review, it has been determined that the domain models arent' as complex as once thought, and auditing can be handled without the complexity of Event Sourcing.
