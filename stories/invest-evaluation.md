# Part I – User Stories

## 3. Evaluate the Quality of User Stories

Each user story was checked against the INVEST criteria:

US01: It is negotiable, valuable, estimable and small. It is not independent because it uses the same booking rules as US03. It is not testable because it is not clear what “times I am able to irrigate” means.

US02: It is negotiable, valuable, estimable, small and testable. It is not independent because it needs the bookings to happen first (US01 and US03).

US03: It is negotiable, valuable, estimable, small and testable. It is not independent because it overlaps with US01 and uses the same check.

US04: It is negotiable and valuable. It is not independent because it needs fault detection, which US08 also uses. It is not estimable or small because it includes both detecting the fault and sending the alert. It is not testable because “as soon as” has no time limit.

US05: It is negotiable and valuable and testable. It is not independent because it needs the schedule from the booking stories. It is not small and s hard to estimate.

US06: It is independent, negotiable and valuable. It is not estimable, small or testable because it is not clear what “fairly” means.

US07: It is negotiable, valuable, estimable, small and testable. It is not independent because it needs the bookings from US01 and US03.

US08: It is negotiable, estimable, small and testable. It is not independent because it uses the same fault detection as US04. It is not valuable because the vendor cant see the record.

US09: It is negotiable and small. It is not independent because it depends on US02. It is not valuable because the one who benefits is the association. It is not estimable or testable because “act on” is too general.

US10: It is negotiable and valuable. It is not independent because it needs the canal data. It is not estimable, small or fully testable because the “national water rules” are not given and it would probably need to be split into multiple stories.

US11: It is negotiable, valuable, estimable and small. It is not independent because it needs the seasonal quota and the canal usage data. It is not fully testable because “close” has no number.
