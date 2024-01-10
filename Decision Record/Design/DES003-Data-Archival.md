# Data Archival

## Context and Problem Statement

I need to decide on what data to archive, and when.

## Considered Options

- No data archival
- Archive visa application data which has not been accessed for a year.
- Archive visa application data which has not been accessed for 5 years.
- Archive all data which has not been accessed for 5 years.

## Decision Outcome

Chosen option: "Archive visa application data which has not been accessed for 5 years", because:

- Authorities or individuals may request this data in the future, so it must be kept.
- Other types of data will not needed in the future, and therefore keeping it will be unnecessary.
- After a time, this data should be archived as "when a database contains a large amount of inactive data, data extract and load processes take much longer to run" (Olson, 2010).
- 5 years is a long enough amount of time to determine that this application data is inactive.

## Consequences

Positive

- We will have the ability to access old visa application data if required.
- This data will not clutter and slow down the main database.

Negative

- Managing archival can be complex, potentially involving data archivists, database archival software, and a complex array of data stores for holding stored data (Olson, 2010).

## Status

Accepted on 9/11/2023
