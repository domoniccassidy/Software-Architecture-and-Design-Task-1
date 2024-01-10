# Database type

## Context and Problem Statement

I need to decide on a type of database to use for storing the AFS system's data

## Considered Options

- Relational Database
- Graph Database
- Document Oriented
- Object Oriented Database

## Decision Outcome

Chosen option: "Relational Database", because:

- The data in the AFS system is mostly structured, which is more tailored to a relational database
- Many non-Relational Databases sacrifice ACID properties, compromising consistency and reliability (Jatana et al., 2012)
- Easy to map objects to entities via Entity Framework
- The schema of a relational database is easy to change, improving maintainability (Jatana et al., 2012).

## Consequences

Positive

- Allows for easily implementing CRUD operations (Jatana et al., 2012)
- The database can be easily hosted on many services such as Azure
- Data accuracy will be enforced via primary and foreign keys (MongoDB, n.d.)

Negative

- The database may be slower due to the complexity of tables, and the links between them (MongoDB, n.d.)
- The database will be expensive to scale if more storage or faster processing is required(MongoDB, n.d.)

## Status

Accepted on 8/11/2023
