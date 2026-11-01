# Part I – User Stories

## 3. Evaluate the Quality of User Stories

Each user story was evaluated against the INVEST criteria. "Yes" means the story meets the criterion, and "Partly" means it meets it with a limitation explained in the notes.

| Story | I | N | V | E | S | T | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| US01 | Partly | Yes | Yes | Yes | Yes | Yes | Shares the booking rules with US03 and US07. Accepted, because splitting it further would leave stories with no value on their own. |
| US02 | Partly | Yes | Yes | Yes | Yes | Yes | Needs turns to exist first (US01), which is accepted because a reminder has no value without a turn. SMS is named because 60% of farmers have basic phones, which is a stated need, not a design choice. |
| US03 | Partly | Yes | Yes | Yes | Yes | Yes | Shares the booking rules with US01. Accepted, because splitting it further would leave stories with no value on their own. |
| US04 | Yes | Yes | Yes | Yes | Yes | Yes | One trigger (a gate fault) and one response (an alert). |
| US05 | Yes | Yes | Yes | Yes | Yes | Yes | Clear rule taken from the kilometer 7 incident. |
| US06 | Yes | Yes | Yes | Partly | Yes | Yes | The report compares water received with each farmer's need, and the method for calculating crop water need is still being researched. Kept as it is, and the estimate will be confirmed once the method is chosen. |
| US07 | Partly | Yes | Yes | Yes | Yes | Yes | Depends on bookings already existing (US01, US03). Accepted, because a clash can only happen once bookings exist. |
| US08 | Yes | Yes | Yes | Yes | Yes | Yes | The fields to record are listed, so it is easy to estimate and test. |
| US09 | Yes | Yes | Yes | Yes | Yes | Yes | Refined (see below). |
| US10 | Yes | Yes | Yes | Yes | Yes | Yes | The rules to check are stated in the Ministry's email. |
| US11 | Yes | Yes | Yes | Yes | Yes | Yes | Refined (see below). |

### Refinements

- **US09 (clarity).** *Before:* "As the SMS gateway provider, I want to report back which messages were not delivered, so that…" The goal described the provider's own action, so it was unclear what the system had to do. *After:* "As the SMS gateway provider, I want the system to act on the delivery reports we send back, so that failures caused by wrong phone numbers are corrected and not blamed on our service."
- **US11 (Estimable and Testable).** The acceptance criteria said the warning is sent at "the warning level", but nobody had defined that level, so the story could not be estimated or tested. *After:* the canal engineer sets the warning level as a percentage of the seasonal share, and AC1 checks the warning against that set level.
