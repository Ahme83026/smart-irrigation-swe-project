 User Stories

| ID | Category | Role | User Story |
| --- | --- | --- | --- |
| US01 | Internal Operational | Farmer | As a farmer, I want to book my irrigation turns at times I am able to irrigate, so that I am not given turns at night. |
| US02 | Internal Operational | Farmer | As a farmer, I want to receive an SMS with my turn times at least a week ahead, so that I can plan my irrigation even with a basic phone. |
| US03 | Internal Operational | Office Clerk | As an office clerk, I want to book turns for farmers who come to the office without giving the same turn to two farmers, so that farmers do not arrive at the same gate at the same time and argue. |
| US04 | Internal Operational | Gatekeeper | As a gatekeeper, I want to be alerted on my phone as soon as a gate fails, even at night, so that I can fix it before water is lost or fields are flooded. |
| US05 | Internal Operational | Canal Engineer | As a canal engineer, I want any gate command outside a scheduled turn to wait for my approval, so that a faulty command cannot break the canal bank again. |
| US06 | Internal Executive | Association Head | As the association head, I want a weekly report comparing the water received at the start, middle and end of the canal, so that I can show farmers that the water is shared fairly. |
| US07 | Internal Executive | Association Head | As the association head, I want to move one of two clashing bookings to another free slot, so that disputes between farmers are settled quickly. |
| US08 | External Operational | Gate and Sensor Vendor | As the gate and sensor vendor, I want every device fault to be recorded with the gate, time, fault type and last reading, so that our technicians can plan repairs at sites far from the office. |
| US09 | External Operational | SMS Gateway Provider | As the SMS gateway provider, I want to report back which messages were not delivered, so that failures caused by wrong phone numbers are corrected and not blamed on our service. |
| US10 | External Executive | Canal Engineer | As a canal engineer, I want to generate a monthly compliance report for the Ministry, so that the inspector can confirm that the national water rules are followed without visiting every site. |
| US11 | External Executive | Canal Engineer | As a canal engineer, I want to be warned when the canal's water use comes close to its seasonal share, so that the canal stays within the limit set by the Water Authority. |

## Stakeholders who do not use the system directly

- **Ministry Irrigation Inspector (External Executive):** The Ministry does not use the system. It already communicates with the association through the Canal Engineer, who receives the season's policy and sends reports back. Her needs are therefore represented by the Canal Engineer role in US10, which produces the compliance report she needs.
- **Water Authority (External Executive):** The Authority does not use the system. It only needs correct usage totals and an early warning near the seasonal limit. These needs are represented by the Canal Engineer role in US11.
- **Gate and Sensor Vendor and SMS Gateway Provider (External Operational):** The companies' staff do not use the system. Their needs are represented through their systems, the smart gates and sensors and the SMS gateway, which exchange data with the system directly (US08 and US09).
