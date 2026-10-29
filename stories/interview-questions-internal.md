# Interview Questions – Internal Stakeholders

**Project:** Smart Irrigation Water Allocation System
**Deliverable:** #2 – Preliminary Activity: Stakeholder Role-Playing
**Prepared by:** Ahmed Hossam (System Analyst, Group #1)
**Session:** 29 October 2026
**Analysts (Group #1):** Ahmed, Ammar
**Users/Stakeholders (Group #2):** Khaled (plays each stakeholder)

## Purpose

These questions guide the simulated requirements elicitation session. For each internal stakeholder category from Deliverable #1, the analysts ask about:

- **Work activities:** what the stakeholder does today
- **Needs and goals:** what they want to achieve
- **Expected interactions:** how they expect to use the system

The questions for the external stakeholders (Vendor, SMS Provider, Ministry Inspector, Water Authority) are prepared by Ammar.

---

## 1. Sayed Eltoukhy – Gatekeeper

**Category:** Internal Operational · **Department:** Field Operations

**Work activities**
1. Can you walk us through a normal working day?
2. How do you check whether each gate is open or closed today?
3. How long does it take you to check the whole canal?

**Problems and needs**
4. What is the hardest part of your job?
5. How do you find out today that a gate has broken?
6. What happens when a gate breaks at night?

**Expected interaction with the system**
7. What information about the gates would you want to see, and when?
8. How quickly do you need to know about a broken gate?
9. Are there times when you need to open or close a gate outside its scheduled turn? What happens then?

**Notes**

- Q1: Starts early and goes along the canal to open and close the gates for each turn. Checks that each gate works and reports any problem to Eng. Shehata.
- Q2: He has to go to each gate and look at it. There is no way to see a gate's status from the office.
- Q3: Checking all 42 gates takes most of the day.
- Q4: Not knowing about a problem until he reaches the gate or a farmer complains.
- Q5: When he passes by the gate or when a farmer complains. Example: a farmer near the head complained that his gate closed 20 minutes early and he lost water.
- Q6: He only learns about it the next morning, so water is lost all night. The canal breach at kilometer 7 also happened at night.
- Q7: Which gates are open or closed right now, and which gates have a fault. He wants to see this at any time of day.
- Q8: Immediately, even at night, on his phone.
- Q9: Yes, for repairs or emergencies. After the breach at kilometer 7, any gate opening outside a turn must be approved by Eng. Shehata.
- Closing: He wants gates that open and close exactly on time.

**Needs found**

- See the status of every gate at any time without walking the canal
- Get an immediate alert on his phone when a gate fails, day or night
- Gates that open and close on time
- A way to open or close a gate outside a turn, with the engineer's approval

---

## 2. Amal Soliman – Office Clerk

**Category:** Internal Operational · **Department:** Association Office

**Work activities**
1. Can you describe what happens in the office on a busy day?
2. How do you book an irrigation turn for a farmer today?
3. What do farmers take with them after booking?

**Problems and needs**
4. What mistakes happen most often when booking turns?
5. What happens when two farmers are given the same turn?
6. What do you do when the internet stops working?

**Expected interaction with the system**
7. What would make booking a turn faster for you?
8. Which farmer details do you need to keep, and how often do they change?
9. What should happen if a farmer asks for a turn that is already taken?

**Notes**

- Q1: Many farmers come at the same time and the queue gets long. She books every turn by hand in the office notebook.
- Q2: She writes the booking in the notebook after checking who already has that day and time. Each farmer tells her the times they prefer and the times they cannot come.
- Q3: Nothing official. She wants to give each farmer a printed paper with their turns.
- Q4: Double bookings, and wrong phone numbers because farmers change their numbers.
- Q5: Both farmers come at the same time and argue. She or Hajj Fathy has to ask one of them to move.
- Q6: The office has one computer and the internet is unstable. When it stops, she goes back to the notebook, but bookings must still continue.
- Q7: Finding the farmer quickly, seeing the free slots straight away, and printing the paper immediately.
- Q8: Name, phone number, whether they use SMS or the app, their plots and gate numbers. Phone numbers change often. Some farmers want a family member, like a son, to get their messages.
- Q9: The system should show her the other free slots right away so she can offer one.
- Closing: Nothing else.

**Needs found**

- Book turns quickly for farmers who come to the office
- Print a paper with each farmer's turns
- Keep booking turns when the internet is down
- Stop double bookings
- Update farmer details, like phone numbers, easily
- See other free slots when the requested one is taken

---

## 3. Mohamed Hegazy and Local Farmers – End-Users / Tail-End Farmers

**Category:** Internal Operational · **Department:** Farmers / Local Community

**Work activities**
1. How do you get your irrigation turn today?
2. At what times of day can you irrigate, and when can you not?
3. What kind of phone do you use?

**Problems and needs**
4. What is your biggest problem with getting water today?
5. As a farmer near the end of the canal, how do you know whether the water reaches you?
6. How do you know how much water you have left?

**Expected interaction with the system**
7. How would you like to be told about your turn? Should anyone else receive these messages?
8. What information would you want before your turn starts?
9. What would you want to know about your field's condition, and when?
10. How do older farmers in your area prefer to receive news?

**Notes**

- Q1: By going to the association office or hearing from other farmers. Sometimes they are told late.
- Q2: During the day. They cannot irrigate at night. One tail farmer was given a turn at 2 am and nobody asked him.
- Q3: A basic phone. About 60 percent of farmers only have basic phones that can receive SMS but no apps.
- Q4: Farms at the end of the canal get less water than farms at the start, so crops are lost.
- Q5: They only know by watching their field. They have no proof, and this causes arguments with farmers at the head.
- Q6: They do not know. Only the office notebook has the records.
- Q7: By SMS. A woman farmer said her son irrigates for her, so he should receive the messages too.
- Q8: The day and time of the turn, at least a week before.
- Q9: When their soil is getting too dry, and whether they can skip a turn if the soil is already wet.
- Q10: Older farmers prefer a phone call or an announcement at the mosque.
- Closing: They want to be asked before being given a night turn.

**Needs found**

- A fair share of water at the end of the canal, with proof that the water reaches them
- Turns at times they can irrigate, not at night
- Messages that work on basic phones (SMS)
- A family member who can also receive their messages
- Know their turns at least a week before
- Know how much water quota they have left
- A warning when their soil is getting too dry
- A phone call or a mosque announcement for older farmers

---

## 4. Eng. Mahmoud Shehata – Canal Engineer & Project Sponsor

**Category:** Internal Operational · **Department:** Canal Management

**Work activities**
1. How is the weekly irrigation schedule prepared today?
2. How do you decide how much water each farmer gets?
3. How do you monitor the water flow in the canal?

**Problems and needs**
4. What happened when the canal broke at kilometer 7, and what caused it?
5. What do you do today when the available water suddenly drops?
6. How do you detect illegal tapping of water?

**Expected interaction with the system**
7. When should the schedule be prepared, and how should it change if the water drops?
8. Which gate operations should need your approval?
9. How quickly do you need to know when the flow becomes too high?
10. What is the minimum share of water each farmer must get in a dry month?

**Notes**

- Q1: He prepares it by hand every week from the bookings and the water available.
- Q2: By each plot's area and crop need, under the Ministry's policy. This summer, food crops like maize and vegetables come before cotton, and rice gets no water. The board wants small farms under 2 feddans protected first, but the Ministry said its policy comes before the board's decisions, and any exception needs written Ministry approval and must be recorded.
- Q3: Through the gatekeeper's reports. He has no live flow data today. The new gates will report flow every 10 minutes.
- Q4: Gate 17 opened fully at night because of a faulty command that was outside any turn. There was no limit on how much a gate can open and no alarm when the flow passed the canal's capacity. The bank broke and four plots were flooded.
- Q5: He changes the schedule the same day and tells everyone affected, by phone or through the office.
- Q6: From the gatekeeper's rounds and farmers' complaints. It is hard to prove.
- Q7: The schedule should be fixed weekly. If the flow drops, it must change the same day and everyone affected must be told.
- Q8: Any gate command outside a scheduled turn.
- Q9: Immediately, on his phone.
- Q10: At least 80 percent of each farmer's calculated need. Nobody gets more than 100 percent until everyone has 80 percent.
- Closing: Gates must keep working on their last schedule if the connection is lost.

**Needs found**

- A fixed weekly schedule that changes the same day if the flow drops, with affected farmers told
- Quotas calculated under the Ministry's policy, with any exception approved by the Ministry in writing and recorded
- Every farmer gets at least 80 percent of their need in a dry month before anyone gets more than 100 percent
- Approve any gate command outside a scheduled turn
- An immediate alarm on his phone when the flow goes above the safe capacity
- Alerts for suspected illegal tapping
- Gates that keep their last schedule if the connection is lost

---

## 5. Hajj Fathy Abdelrazek – Association Head

**Category:** Internal Executive · **Department:** Association Board

**Work activities**
1. What are your main responsibilities as head of the association?
2. How do you settle disputes between farmers today?
3. How are fees, credits and penalties applied today?

**Problems and needs**
4. What is your biggest worry about how water is shared?
5. How can you show farmers that the sharing is fair between the start and the end of the canal?
6. What happens today when two bookings clash?

**Expected interaction with the system**
7. What information would you need to prove that allocation is fair, and how often?
8. When should farmers be allowed to swap turns?
9. How should fees, credits and penalties be applied so that everyone is treated the same?
10. The board wants quotas to be public, but some farmers do not want neighbours to know their land size. How should this be handled?

**Notes**

- Q1: Keeping the peace between farmers, leading the board, settling disputes and applying the bylaws.
- Q2: He meets both farmers and asks one of them to move. Every summer, people at the tail shout at people at the head.
- Q3: Fees are paid every season, and farmers with unpaid fees for more than one season cannot book. Taking water outside a turn is a violation: first a written warning, then a 500 EGP fine, then a two-week suspension of turns. Farmers who save water should get priority next season.
- Q4: Farmers at the end of the canal getting less water, which leads to fights.
- Q5: Today he cannot, because there are no clear records. The system must be fair, and people must see that it is fair.
- Q6: He or the office decides who moves, and the farmers often argue.
- Q7: A report comparing the water received at the start, middle and end of the canal. He wants it every week during summer.
- Q8: When both farmers agree.
- Q9: Using the same bylaw rules for everyone, applied by the system without exceptions made by hand.
- Q10: He suggests showing each farmer's share as a percentage of their need, without showing land size.
- Closing: SMS is fine for most farmers, but older farmers prefer a phone call or the mosque announcement.

**Needs found**

- Reports that show fairness between the start and the end of the canal
- Move turns when bookings clash
- Allow farmers to swap turns if both agree
- Fees, credits and penalties applied the same way to everyone, following the bylaws
- Stop farmers with fees unpaid for more than one season from booking
- Show fairness to farmers without showing each farmer's land size
- Reach older farmers by phone call or the mosque announcement

---

## Closing question for every stakeholder

- Is there anything else you need from the system that we did not ask about?
