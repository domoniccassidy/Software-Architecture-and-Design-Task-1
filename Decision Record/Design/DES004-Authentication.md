# Authentication

## Context and Problem Statement

I need to decide on an authentication policy for visa applicants.

## Considered Options

- No authentication required
- An email and password stored in plaintext
- An email nad password stored with the password being salted then hashed.
- An email and password with the password being salted then hashed incorporating two factor authentication (an email or text sent to the applicant providing a code they must use when they log in from a new device)

## Decision Outcome

Chosen option: "An email and password with the password being salted then hashed incorporating two factor authentication", because:

- Authentication must be required to prove the identity of the applicant
- Storing the password in plaintext would harm the Confidentiality and Integrity of the system, as if someone was to view the password, they could log onto that applicants account, and view/update their application data
- Two-factor authentication provides a strong defense against remote impersonation attacks (Reese, 2018), as if a bad actor were to retrieve the password of a user, this would not be enough for them to get into the applicant's account to view update application data.

## Consequences

Positive

- The system will be able to prove the identity of all applicants.
- The system will adhere to the Confidentiality security principle
- The system will adhere to the Integrity security principle

Negative

- Users often find two-factor authentication too inconvenient to be worth the additional security (Reese, 2018).

## Status

Accepted on 14/11/2023
