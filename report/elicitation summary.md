# Requirements Elicitation Session Summary


## Session setup

- **Group #1 – System Analysts:** Ahmed Hossam and Ammar Mohamed Nabil
- **Group #2 – Users/Stakeholders:** Khaled Elsayed Elsayegh, who played each stakeholder from Deliverable #1

## Stakeholder roles represented

| Stakeholder | Role | Category |
| --- | --- | --- |
| Sayed Eltoukhy | Gatekeeper | Internal Operational |
| Amal Soliman | Office Clerk | Internal Operational |
| Mohamed Hegazy and Local Farmers | End-Users / Tail-End Farmers | Internal Operational |
| Eng. Mahmoud Shehata | Canal Engineer & Project Sponsor | Internal Operational |
| Hajj Fathy Abdelrazek | Association Head | Internal Executive |
| IoT Sensor & Smart Gate Vendor | Hardware Supplier & Maintainer | External Operational |
| SMS Gateway Provider | Communication Service | External Operational |
| Eng. Doaa Mostafa | Ministry Irrigation Inspector | External Executive |
| Water Authority | Regional Water Allocation Body | External Executive |

## Key questions raised

- **Gatekeeper:** How do you find out that a gate has broken? How quickly do you need to know?
- **Office Clerk:** How do you book a turn for a farmer today? What do you do when the internet stops working?
- **Farmers:** When can you irrigate, and when can you not? How do you know whether the water reaches you?
- **Canal Engineer:** What caused the breach at kilometer 7? Which gate operations should need your approval?
- **Association Head:** How can you show farmers that the sharing is fair? When should farmers be allowed to swap turns?
- **Vendor:** What happens when a gate loses its connection? What should be checked before a command is sent to a gate?
- **SMS Provider:** What usually causes messages to fail? How should the system know a message was not delivered?
- **Ministry Inspector:** How do the board's wishes fit with the Ministry's policy? How should exceptions be approved?
- **Water Authority:** What usage figures do you need, and how often? What happens if the seasonal share is cut?

## Requirements identified

**Booking and turns**
1. Farmers book turns in the app or at the office, giving the slots they prefer and the slots they cannot use. *(Farmers, Office Clerk)*
2. A slot cannot be booked twice, and when a slot is taken the clerk sees the other free slots. *(Office Clerk)*
3. The office can keep booking turns when the internet is down. *(Office Clerk)*
4. The office can print a paper with each farmer's turns. *(Office Clerk)*
5. Farmer details, such as phone numbers, are easy to update, and a family member can receive a farmer's messages. *(Office Clerk, Farmers)*
6. Farmers with fees unpaid for more than one season cannot book. *(Association Head)*
7. The head can move turns when bookings clash, and farmers can swap turns if both agree. *(Association Head)*
8. Farmers are not given night turns without being asked. *(Farmers)*

**Allocation and scheduling**
9. Quotas follow the Ministry's policy, and crops it does not allow, such as rice this summer, get no water. *(Ministry Inspector, Canal Engineer)*
10. Exceptions need written Ministry approval and are recorded with who approved them and when. Each quota records the policy used. *(Ministry Inspector, Canal Engineer)*
11. In a dry month, every farmer gets at least 80% of their need before anyone gets more than 100%. *(Canal Engineer)*
12. The schedule is fixed weekly and changed the same day if the flow drops, and affected farmers are told. *(Canal Engineer)*
13. The seasonal share is entered at the start of each season, and quotas are recalculated if it changes. *(Water Authority)*

**Gates and alerts**
14. The status of every gate can be seen at any time, and gates open and close on time. *(Gatekeeper)*
15. Gate commands outside a scheduled turn need the engineer's approval, and gates cannot open past a safe limit. *(Canal Engineer, Gatekeeper, Vendor)*
16. Immediate phone alerts, day or night: gate faults go to the gatekeeper, and high flow and suspected illegal tapping go to the engineer. *(Gatekeeper, Canal Engineer)*
17. Fault reports show the gate, time, fault type and last reading, with few false alarms. *(Vendor)*
18. Gates keep their last schedule if the connection is lost. *(Canal Engineer, Vendor)*

**Notifications**
19. Farmers get SMS messages about their turns at least a week ahead, any changes, and their remaining water. *(Farmers)*
20. Farmers are warned when their soil is too dry and told when they can skip a turn. *(Farmers)*
21. Failed messages are found through delivery reports and sent again, and the system can receive farmers' SMS replies. *(SMS Provider)*
22. Older farmers are told by phone call or a mosque announcement. *(Farmers, Association Head)*

**Fairness, fees and reports**
23. A weekly report in summer compares the water received at the start, middle and end of the canal. *(Association Head, Farmers)*
24. Fees, credits and bylaw penalties apply the same way to everyone: a written warning, then a 500 EGP fine, then a two-week suspension. *(Association Head)*
25. Each farmer's share is shown as a percentage of their need, without showing land size. *(Association Head)*
26. Water use is measured from the gates' flow readings, with an early warning before the seasonal share is exceeded. *(Water Authority)*
27. The Ministry gets monthly reports on water used, the policy applied and the crops planted. *(Ministry Inspector)*
