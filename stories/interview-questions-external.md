# Interview Questions – External Stakeholders

**Project:** Smart Irrigation Water Allocation System
**Deliverable:** #2 – Preliminary Activity: Stakeholder Role-Playing
**Prepared by:** Ammar Mohamed Nabil (System Analyst, Group #1)
**Session:** 29 October 2026
**Analysts (Group #1):** Ahmed, Ammar
**Users/Stakeholders (Group #2):** Khaled (plays each stakeholder)

## Purpose

These questions guide the simulated requirements elicitation session. For each external stakeholder category from Deliverable #1, the analysts ask about:

- **Work activities:** what the stakeholder does today
- **Needs and goals:** what they want to achieve
- **Expected interactions:** how they expect to use or connect to the system

The questions for the internal stakeholders (Gatekeeper, Office Clerk, Farmers, Canal Engineer, Association Head) are prepared by Ahmed.

---

## 1. IoT Sensor & Smart Gate Vendor – Hardware Supplier & Maintainer

**Category:** External Operational · **Department:** Field Telemetry Infrastructure

**Work activities**
1. What equipment have you supplied, and what can it do?
2. How do the gates and sensors send their data?
3. How do you maintain the equipment in the field?

**Problems and needs**
4. What problems happen most often with the gates and sensors?
5. What happens when a gate loses its connection?
6. What did you learn from the Gate 17 failure at kilometer 7?

**Expected interaction with the system**
7. What information do you need from the system to fix a fault quickly?
8. What should the system check before it sends a command to a gate?
9. How should the system tell real faults apart from false alarms?

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
- Closing: A maintenance plan that is realistic for sites far from the office.

**Needs found**

- A clear specification of the commands and data the gates and sensors use
- Detailed fault reports with the gate, time, fault type and last reading
- Gate commands outside a scheduled turn rejected unless an engineer approves them
- A safe limit on how far a gate can open
- Gates that keep their last schedule when the connection is lost
- Few false alarms
- A realistic maintenance plan for remote sites

---

## 2. SMS Gateway Provider – Communication Service

**Category:** External Operational · **Department:** External Telecom Service

**Work activities**
1. How will the association's messages be sent through your service?
2. How many messages should you expect from the association?
3. What information do you need for each message?

**Problems and needs**
4. What usually causes messages to fail?
5. What happens when a farmer changes their phone number?
6. What happens when the network is busy or down?

**Expected interaction with the system**
7. How should the system find out that a message was not delivered?
8. How should replies from farmers be passed to the system?
9. What should the contract with the association cover?

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
- Closing: Problems caused by wrong numbers should not be blamed on the provider.

**Needs found**

- Correct, up to date phone numbers for every farmer
- A predictable number of messages and a clear contract
- Delivery reports, so failed messages can be found and sent again
- Two-way SMS, so farmers' replies reach the system
- A stable connection between the system and the provider

---

## 3. Eng. Doaa Mostafa – Ministry Irrigation Inspector

**Category:** External Executive · **Department:** Ministry of Water Resources & Irrigation

**Work activities**
1. What does the Ministry check when it inspects a canal?
2. How is the allocation policy chosen and sent to the association each season?
3. How do you get information about each canal today?

**Problems and needs**
4. What problems do you find most often during inspections?
5. The board wants to protect small farms under 2 feddans first. How should that work with the Ministry's policy?
6. What should happen when an association needs an exception to the policy?

**Expected interaction with the system**
7. Which allocation policies must the system be able to apply?
8. What reports would you need from the system, and how often?
9. How should exceptions be approved and recorded in the system?

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
- Closing: Each farmer's quota should show which policy was used to calculate it.

**Needs found**

- Apply whichever allocation policy the Ministry chooses
- No allocation for crops the Ministry does not allow, such as rice this summer
- Exceptions only with written Ministry approval, recorded with who approved and when
- Regional reports she can trust without visiting every site
- A record of the policy used for each farmer's quota

---

## 4. Water Authority – Regional Water Allocation Body

**Category:** External Executive · **Department:** Public Water Sector

**Work activities**
1. How is the seasonal water share for the branch canal decided?
2. How is the seasonal share given to the association?
3. How do you check how much water each canal uses today?

**Problems and needs**
4. What happens when a canal uses more than its share?
5. What makes today's usage figures hard to trust?
6. Can the seasonal share change during the season?

**Expected interaction with the system**
7. What usage figures do you need from the system, and how often?
8. When should you be warned that usage is close to the limit?
9. What should happen in the system if the share is cut during the season?

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
- Closing: Nothing else.

**Needs found**

- Accurate totals of water taken, measured from the gates' flow readings
- An early warning before the canal goes over its seasonal share
- A way to enter the seasonal share at the start of each season
- Quotas and the schedule recalculated if the share changes during the season

---

## Closing question for every stakeholder

- Is there anything else you need from the system that we did not ask about?
