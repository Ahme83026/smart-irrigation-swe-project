# Part I – User Stories

## 2. Define Acceptance Criteria

Each acceptance criterion uses the Given–When–Then format: **Given** is the context or precondition, **When** is the action that is carried out, and **Then** is the observable outcome and expected result. **And** adds a further expected result.

### US01 – Book irrigation turns at times the farmer can irrigate

**AC1**
- **Given:** a farmer has remaining quota and has given his preferred and blocked slots
- **When:** he books a turn in one of his preferred daytime slots
- **Then:** the turn is assigned to him
- **And:** the confirmed day and time are shown

**AC2**
- **Given:** a night slot is one of the farmer's blocked slots
- **When:** the schedule is assigned
- **Then:** that slot is not given to him

**AC3**
- **Given:** the farmer's quota for the season is used up
- **When:** he tries to book a turn
- **Then:** the booking is refused
- **And:** his remaining quota is shown as zero

### US02 – Receive turn times by SMS a week ahead

**AC1**
- **Given:** a farmer who uses SMS has a turn assigned
- **When:** the weekly schedule is fixed, at least one week before the turn
- **Then:** he receives an SMS with the day, time and gate number of his turn

**AC2**
- **Given:** the farmer's turn is changed after the SMS was sent
- **When:** the schedule is updated
- **Then:** he receives a new SMS with the changed turn

**AC3**
- **Given:** the farmer has added a family member as a second contact
- **When:** the SMS is sent
- **Then:** the family member receives the same SMS

### US03 – Book turns at the office without double bookings

**AC1**
- **Given:** a farmer is at the office and the slot he wants is free
- **When:** the clerk books the slot for him
- **Then:** the turn is saved for that farmer
- **And:** the slot is no longer shown as free

**AC2**
- **Given:** the slot is already booked by another farmer
- **When:** the clerk tries to book it
- **Then:** the booking is rejected
- **And:** the other free slots are shown

**AC3**
- **Given:** the farmer has unpaid fees for more than one season
- **When:** the clerk tries to book a turn for him
- **Then:** the booking is refused
- **And:** the reason is shown

### US04 – Alert the gatekeeper when a gate fails

**AC1**
- **Given:** a gate reports a fault
- **When:** the system receives the report
- **Then:** the gatekeeper gets a phone alert with the gate number, its location and the fault type

**AC2**
- **Given:** the fault happens at night
- **When:** the report is received
- **Then:** the alert is sent immediately
- **And:** it is not held until the morning

**AC3**
- **Given:** a faulty gate has been repaired
- **When:** the gate reports that it is working again
- **Then:** the alert is closed
- **And:** the gate is shown as working

### US05 – Approve gate commands outside a scheduled turn

**AC1**
- **Given:** a gate command does not match any scheduled turn
- **When:** the command is sent
- **Then:** the gate does not move until the canal engineer approves it

**AC2**
- **Given:** a command is waiting for approval
- **When:** the canal engineer approves it
- **Then:** the command is sent to the gate
- **And:** it is recorded with his name and the time

**AC3**
- **Given:** a command is waiting for approval
- **When:** the canal engineer rejects it
- **Then:** the command is cancelled
- **And:** the person who requested it is told

### US06 – Weekly fairness report

**AC1**
- **Given:** a week in the summer season has ended
- **When:** the weekly report is produced
- **Then:** it shows the water received against the need for the start, middle and end of the canal

**AC2**
- **Given:** in a dry month, some farmers received less than 80% of their need
- **When:** the report is produced
- **Then:** those farmers are highlighted in the report

**AC3**
- **Given:** the report is shown to farmers
- **When:** it is printed or displayed
- **Then:** each share is shown as a percentage of need
- **And:** no land sizes appear

### US07 – Move clashing bookings

**AC1**
- **Given:** two bookings clash on the same gate and time
- **When:** the association head moves one of them to a free slot
- **Then:** both farmers keep a turn
- **And:** the moved farmer is told about the new time

**AC2**
- **Given:** no free slot is left on that day
- **When:** the association head tries to move a booking
- **Then:** the free slots on the following days are shown instead

### US08 – Record device faults with details

**AC1**
- **Given:** a gate or sensor reports a fault
- **When:** the fault is recorded
- **Then:** the record shows the device, the time, the fault type and the last reading

**AC2**
- **Given:** a device sends one unusual reading
- **When:** the reading is received
- **Then:** no fault is raised unless the next reading confirms it

### US09 – Act on SMS delivery reports

**AC1**
- **Given:** a message has been sent to a farmer
- **When:** the provider reports that it was not delivered
- **Then:** the failure is recorded
- **And:** the message is sent again

**AC2**
- **Given:** a resent message fails again
- **When:** the second failure is reported
- **Then:** the farmer is flagged so the clerk can check his phone number

### US10 – Monthly compliance report for the Ministry

**AC1**
- **Given:** a month in the summer season has ended
- **When:** the canal engineer generates the compliance report
- **Then:** it shows the water used, the allocation policy applied and the crops planted

**AC2**
- **Given:** a plot is planted with rice this summer
- **When:** the report is generated
- **Then:** the plot is shown with no water allocated

**AC3**
- **Given:** the Ministry has approved an exception in writing
- **When:** the report is generated
- **Then:** the exception is listed with who approved it and the date

### US11 – Warning near the seasonal share

**AC1**
- **Given:** the seasonal share has been entered and the canal engineer has set the warning level as a percentage of it
- **When:** the water used reaches that level
- **Then:** the canal engineer is warned with the water used so far and the amount remaining

**AC2**
- **Given:** the Water Authority changes the seasonal share during the season
- **When:** the new share is entered
- **Then:** the warning level is recalculated using the new share
