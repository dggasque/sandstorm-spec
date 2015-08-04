# Person

A person contains all the identifying information for a single individual.

| field        | description (optional)
|--------------|-------------------------------------------
| firstName    |
| lastName     |
| dateOfBirth  |
| addressLine1 |
| addressLine2 |
| city         |
| state        |
| country      |
| postalCode   |
| control      | A hash representing the unique person
| verified     | Whether or not the person has been verified


## Additional Field Details

### control

The control will be calculated based on `firstName`, `lastName`, `dateOfBirth`, concatenated, lowercased, and having all non-alphanumeric characters removed.

### verified

A person will be verified based on a variety of checks, mostly based on peer verification, i.e. someone met you at an organization meeting.  Verification may be revoked at any time by admins.
