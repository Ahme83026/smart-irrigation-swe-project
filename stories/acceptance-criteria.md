# Part I – User Stories

## 2. Define Acceptance Criteria

| Story | AC | Given | When | Then |
| --- | --- | --- | --- | --- |
| US01 | AC1 | A farmer has remaining quota and has given his preferred and blocked slots | He books a turn in one of his preferred daytime slots | The turn is assigned to him and the confirmed day and time are shown |
| US01 | AC2 | A night slot is one of the farmer's blocked slots | The schedule is assigned | That slot is not given to him |
| US01 | AC3 | The farmer's quota for the season is used up | He tries to book a turn | The booking is refused and his remaining quota is shown as zero |
| US02 | AC1 | A farmer who uses SMS has a turn assigned | The weekly schedule is fixed, at least one week before the turn | He receives an SMS with the day, time and gate number of his turn |
| US02 | AC2 | The farmer's turn is changed after the SMS was sent | The schedule is updated | He receives a new SMS with the changed turn |
| US02 | AC3 | The farmer has added a family member as a second contact | The SMS is sent | The family member receives the same SMS |
| US03 | AC1 | A farmer is at the office and the slot he wants is free | The clerk books the slot for him | The turn is saved for that farmer and the slot is no longer shown as free |
| US03 | AC2 | The slot is already booked by another farmer | The clerk tries to book it | The booking is rejected and the other free slots are shown |
| US03 | AC3 | The farmer has unpaid fees for more than one season | The clerk tries to book a turn for him | The booking is refused and the reason is shown |
| US04 | AC1 | A gate reports a fault | The system receives the report | The gatekeeper gets a phone alert with the gate number, its location and the fault type |
| US04 | AC2 | The fault happens at night | The report is received | The alert is sent immediately and is not held until the morning |
| US04 | AC3 | A faulty gate has been repaired | The gate reports that it is working again | The alert is closed and the gate is shown as working |
| US05 | AC1 | A gate command does not match any scheduled turn | The command is sent | The gate does not move until the canal engineer approves it |
| US05 | AC2 | A command is waiting for approval | The canal engineer approves it | The command is sent to the gate and recorded with his name and the time |
| US05 | AC3 | A command is waiting for approval | The canal engineer rejects it | The command is cancelled and the person who requested it is told |
| US06 | AC1 | A week in the summer season has ended | The weekly report is produced | It shows the water received against the need for the start, middle and end of the canal |
| US06 | AC2 | In a dry month, some farmers received less than 80% of their need | The report is produced | Those farmers are highlighted in the report |
| US06 | AC3 | The report is shown to farmers | It is printed or displayed | Each share is shown as a percentage of need and no land sizes appear |
| US07 | AC1 | Two bookings clash on the same gate and time | The association head moves one of them to a free slot | Both farmers keep a turn and the moved farmer is told about the new time |
| US07 | AC2 | No free slot is left on that day | The association head tries to move a booking | The free slots on the following days are shown instead |
| US08 | AC1 | A gate or sensor reports a fault | The fault is recorded | The record shows the device, the time, the fault type and the last reading |
| US08 | AC2 | A device sends one unusual reading | The reading is received | No fault is raised unless the next reading confirms it |
| US09 | AC1 | A message has been sent to a farmer | The provider reports that it was not delivered | The failure is recorded and the message is sent again |
| US09 | AC2 | A resent message fails again | The second failure is reported | The farmer is flagged so the clerk can check his phone number |
| US10 | AC1 | A month in the summer season has ended | The canal engineer generates the compliance report | It shows the water used, the allocation policy applied and the crops planted |
| US10 | AC2 | A plot is planted with rice this summer | The report is generated | The plot is shown with no water allocated |
| US10 | AC3 | The Ministry has approved an exception in writing | The report is generated | The exception is listed with who approved it and the date |
| US11 | AC1 | The seasonal share has been entered and the canal engineer has set the warning level as a percentage of it | The water used reaches that level | The canal engineer is warned with the water used so far and the amount remaining |
| US11 | AC2 | The Water Authority changes the seasonal share during the season | The new share is entered | The warning level is recalculated using the new share |
