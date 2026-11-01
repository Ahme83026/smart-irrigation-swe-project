# Interview Agenda – External Stakeholders

## 1. IoT Sensor & Smart Gate Vendor – Hardware Supplier & Maintainer

**Category:** External Operational · **Department:** Field Telemetry Infrastructure

### Setting

- **Objective of interview:** Understand how the gates and sensors work and are maintained, and what the vendor needs from the system
- **Date, time and location:** 29 October 2026, 8:00 PM, online via Google Meet
- **User participants:** IoT Sensor and Smart Gate Vendor (role played by Khaled Elsayed Elsayegh)
- **Project team participants:** Ammar Mohamed Nabil (asked the questions) and Ahmed Hossam (took notes)

### Interview/Discussion

1. What equipment have you supplied, and what can it do?
2. How do the gates and sensors send their data?
3. How do you maintain the equipment in the field?
4. What problems happen most often with the gates and sensors?
5. What happens when a gate loses its connection?
6. What did you learn from the Gate 17 failure at kilometer 7?
7. What information do you need from the system to fix a fault quickly?
8. What should the system check before it sends a command to a gate?
9. How should the system tell real faults apart from false alarms?
10. Is there anything else you need from the system that we did not ask about?

**Notes**

- Q1: 42 smart gates with solar panels and 320 soil moisture sensors. Each gate accepts open and close commands and reports its flow every 10 minutes.
- Q2: Sensors send a reading every hour by LoRa radio to a gateway in the association office. Gates report flow every 10 minutes.
- Q3: A technician visits the gates when a fault is reported. The sites are far apart along the canal, so each visit takes time.
- Q4: Gates losing their connection, and sensors that stop sending readings.
- Q5: The gate keeps working on its last schedule until the connection comes back.
- Q6: Gate 17 accepted a command that was outside any scheduled turn, and there was no limit on how far a gate can open.
- Q7: The gate number, the time, the type of fault and the last flow reading.
- Q8: That the command matches a scheduled turn, or that an engineer has approved it, and that the gate does not open more than a safe limit.
- Q9: By checking a fault over more than one reading before raising an alarm.
- Q10: A maintenance plan that is realistic for sites far from the office.

### Follow-Up

**Important decisions or answers to questions**

- A clear specification of the commands and data the gates and sensors use
- Detailed fault reports with the gate, time, fault type and last reading
- Gate commands outside a scheduled turn rejected unless an engineer approves them
- A safe limit on how far a gate can open
- Gates that keep their last schedule when the connection is lost
- Few false alarms
- A realistic maintenance plan for remote sites

**Follow-up questions (information, inputs and outputs)**

- **Q11. What information do you use?** The schedule for each gate and any commands approved by the canal engineer.
- **Q12. What inputs do you use?** Open and close commands from the system.
- **Q13. What outputs do you produce?** Flow readings from the gates every 10 minutes, soil moisture readings every hour, and fault reports.

**Open items not resolved:** None

---

## 2. SMS Gateway Provider – Communication Service

**Category:** External Operational · **Department:** External Telecom Service

### Setting

- **Objective of interview:** Understand how messages will be delivered to farmers, and what the SMS provider needs from the system
- **Date, time and location:** 29 October 2026, 8:00 PM, online via Google Meet
- **User participants:** SMS Gateway Provider (role played by Khaled Elsayed Elsayegh)
- **Project team participants:** Ammar Mohamed Nabil (asked the questions) and Ahmed Hossam (took notes)

### Interview/Discussion

1. How will the association's messages be sent through your service?
2. How many messages should you expect from the association?
3. What information do you need for each message?
4. What usually causes messages to fail?
5. What happens when a farmer changes their phone number?
6. What happens when the network is busy or down?
7. How should the system find out that a message was not delivered?
8. How should replies from farmers be passed to the system?
9. What should the contract with the association cover?
10. Is there anything else you need from the system that we did not ask about?

**Notes**

- Q1: The system sends each message to the provider, which delivers it as an SMS to the farmer's phone.
- Q2: The association has about 900 farmers, and about 60 percent of them can only receive SMS. Each farmer gets at least one message a week, and more in summer and when the schedule changes.
- Q3: The phone number and the message text. Messages must be short.
- Q4: Wrong or old phone numbers. A farmer complained that he did not get the SMS because he had a new number.
- Q5: Messages keep going to the old number until the association updates it.
- Q6: Messages are delayed and sent again later.
- Q7: The provider sends back a delivery report for each message, so the system can see which ones failed and send them again.
- Q8: The service can pass every SMS reply from a farmer back to the system.
- Q9: The expected number of messages, the price, and the delivery reports.
- Q10: Problems caused by wrong numbers should not be blamed on the provider.

### Follow-Up

**Important decisions or answers to questions**

- Correct, up to date phone numbers for every farmer
- A predictable number of messages and a clear contract
- Delivery reports, so failed messages can be found and sent again
- Two-way SMS, so farmers' replies reach the system
- A stable connection between the system and the provider

**Follow-up questions (information, inputs and outputs)**

- **Q11. What information do you use?** The expected number of messages and the terms of the contract.
- **Q12. What inputs do you use?** The phone number and the text of each message.
- **Q13. What outputs do you produce?** SMS messages delivered to farmers, a delivery report for each message, and farmers' replies.

**Open items not resolved:** None

---

## 3. Eng. Doaa Mostafa – Ministry Irrigation Inspector

**Category:** External Executive · **Department:** Ministry of Water Resources & Irrigation

### Setting

- **Objective of interview:** Understand the Ministry's allocation rules and how compliance should be checked and reported
- **Date, time and location:** 29 October 2026, 8:00 PM, online via Google Meet
- **User participants:** Eng. Doaa Mostafa, Ministry Irrigation Inspector (role played by Khaled Elsayed Elsayegh)
- **Project team participants:** Ammar Mohamed Nabil (asked the questions) and Ahmed Hossam (took notes)

### Interview/Discussion

1. What does the Ministry check when it inspects a canal?
2. How is the allocation policy chosen and sent to the association each season?
3. How do you get information about each canal today?
4. What problems do you find most often during inspections?
5. The board wants to protect small farms under 2 feddans first. How should that work with the Ministry's policy?
6. What should happen when an association needs an exception to the policy?
7. Which allocation policies must the system be able to apply?
8. What reports would you need from the system, and how often?
9. How should exceptions be approved and recorded in the system?
10. Is there anything else you need from the system that we did not ask about?

**Notes**

- Q1: That the canal follows the national water-saving rules and the allocation policy for the season.
- Q2: The Ministry chooses the policy and tells the canal engineer by email. This summer, rice is not allowed in the district, and food crops such as maize and vegetables get priority over cotton and other cash crops.
- Q3: By visiting the sites, which takes a lot of time.
- Q4: Crops planted that the policy does not allow, and canals using more water than they should.
- Q5: The Ministry's policy is above the board's decision. Protecting small farms is only possible as an exception.
- Q6: Any exception must be approved by the Ministry in writing and recorded.
- Q7: Food crops first, the same percentage cut for everyone, or protection for small farms. Plots planted with rice get no allocation this summer.
- Q8: Reports she can trust without visiting every site: water used, the policy applied and the crops planted. Every month during summer.
- Q9: Only the Ministry approves an exception. The system records the approval, who gave it and the date.
- Q10: Each farmer's quota should show which policy was used to calculate it.

### Follow-Up

**Important decisions or answers to questions**

- Apply whichever allocation policy the Ministry chooses
- No allocation for crops the Ministry does not allow, such as rice this summer
- Exceptions only with written Ministry approval, recorded with who approved and when
- Regional reports she can trust without visiting every site
- A record of the policy used for each farmer's quota

**Follow-up questions (information, inputs and outputs)**

- **Q11. What information do you use?** The national water rules, and each canal's water use and crops planted.
- **Q12. What inputs do you use?** Reports from the canal engineer and findings from her site visits.
- **Q13. What outputs do you produce?** The allocation policy for each season, sent by email, and written approvals for exceptions.

**Open items not resolved:** See open item 2.

---

## 4. Water Authority – Regional Water Allocation Body

**Category:** External Executive · **Department:** Public Water Sector

### Setting

- **Objective of interview:** Understand how the seasonal share is set and what usage information the Water Authority needs
- **Date, time and location:** 29 October 2026, 8:00 PM, online via Google Meet
- **User participants:** Water Authority (role played by Khaled Elsayed Elsayegh)
- **Project team participants:** Ammar Mohamed Nabil (asked the questions) and Ahmed Hossam (took notes)

### Interview/Discussion

1. How is the seasonal water share for the branch canal decided?
2. How is the seasonal share given to the association?
3. How do you check how much water each canal uses today?
4. What happens when a canal uses more than its share?
5. What makes today's usage figures hard to trust?
6. Can the seasonal share change during the season?
7. What usage figures do you need from the system, and how often?
8. When should you be warned that usage is close to the limit?
9. What should happen in the system if the share is cut during the season?
10. Is there anything else you need from the system that we did not ask about?

**Notes**

- Q1: From the total water available in the region for the season.
- Q2: At the start of each season, the Authority tells the association the total water available for the branch canal.
- Q3: From reports sent by the canal engineer, which are written by hand.
- Q4: Other canals in the region get less water.
- Q5: The figures are collected by hand and are not measured at the gates.
- Q6: Yes, if the water level in the region drops.
- Q7: The total water taken by the canal, measured at the gates. Every week during summer.
- Q8: Well before the limit, so the association has time to act.
- Q9: The quotas and the schedule should be recalculated, and the farmers told.
- Q10: Nothing else.

### Follow-Up

**Important decisions or answers to questions**

- Accurate totals of water taken, measured from the gates' flow readings
- An early warning before the canal goes over its seasonal share
- A way to enter the seasonal share at the start of each season
- Quotas and the schedule recalculated if the share changes during the season

**Follow-up questions (information, inputs and outputs)**

- **Q11. What information do you use?** The total water available in the region for the season.
- **Q12. What inputs do you use?** The usage reports sent by the canal engineer.
- **Q13. What outputs do you produce?** The seasonal share for the branch canal, given to the association at the start of each season.

**Open items not resolved:** See open item 3.

---

## Open Items List

| ID | Issue title | Date identified | Target end date | Responsible project person | User contact | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| 2 | Protecting small farms | 29-10-2026 | To be agreed | Ammar Mohamed Nabil | Eng. Doaa Mostafa | The board wants small farms under 2 feddans protected first. This is only possible as an exception with written Ministry approval, and no approval has been requested yet. |
| 3 | Warning level near the seasonal share | 29-10-2026 | To be agreed | Ammar Mohamed Nabil | Water Authority | The Authority wants a warning "well before the limit", but the exact level has not been agreed. |
