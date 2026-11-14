# Table

| **Event ID** | **Event Description** | **Event Type** | **Triggering actors / condition** | **Corresponding Use Case** |
|:----:|:----:|:----:|:---:|:---:|
|E01 | Local Farmer wants to register his corps | External | Local farmer |Register corps |
|E02 | Local Farmer changes his contact details | External | Local farmer |Update farmer details |
|E03 | Local Farmer changes / drops plot | External | Local farmer |Adjust farmer plots |
|E04 | Turns are assigned to local farmers | External | Assosciation head / Local farmer |Assign turns to local farmers |
|E05 | Water authority gives total seasonal water | External | Water Authority |Give total available seasonal water |
|E06 | Local Farmer wants to choose slot | External | Local farmer |Book irrigation turn |
|E07 | New Quota Calculation | Include | At the start of a new season |Calculate season quota |
|E08 | Local farmers are informed of new seasonal quota | Temporal | At the start of a new season |Notify local farmers their seasonal quota |
|E09 | Local Farmer exceeds quota | State | At the end of each season |Check used quota by local farmer |
|E10 | Local Farmer saved quota | State | At the end of each season |Check used quota by local farmer |
|E11 | Water passing on plots | Temporal | During every turn (maybe every hour not specified) |skip wet plot |
|E12 | Schedule conflict | State | Schedule |Negotiate with local farmer |
|E13 | Dry month | State | Total seasonal water / total available water of the season is reduced due to dry month |Apply ministry policy |
|E14 | Internet Outage | State | Telecom service / application is offline so online booking is unavailable | Allow farmers to book through office |
|E15 | Water demand > Supply | State | water demand / total available water of the season is limited | Apply ministry policy |
|E16 | Smart Gate mulfunctioning | State | Gate / Water isn't delivered or flows in unexpected times | Report gate malfunction |
|E17 | Soil moisture report | temporal | Sensor / Every hour the sensor reports soil moisture | Report soil moisture |

### Notes

1. E15's & E05's UCs could be merged to one use case
2. E013's UC could be merged too with E15's & E05's if we assumed that we would know at the start of the season that a dry month will occur
3. update farmer details triggered UC for E02 might be ignored because the significant point is recalculating new quota for his change rather than updating the new plot in the info
