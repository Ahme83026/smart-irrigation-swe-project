# Table

| **Event ID** | **Event Description** | **Event Type** | **Triggering actor / condition** | **Corresponding Use Case** |
|:----:|:----:|:----:|:---:|:---:|
|E01 | Local Farmer changes his contact details | External | Local farmer |update farmer details |
|E02 | Local Farmer changes / drops plot | External | Local farmer |update farmer details / recalculate new quota |
|E03 | Water authority gives total seasonal water | External | Water Authority |compare supply and demand |
|E04 | Local Farmer wants to choose slot | External | Local farmer |Book irrigation turn |
|E05 | New Quota Calculation | Temporal | At the start of a new season |calculate season quota |
|E06 | Local Farmer exceeds quota | Temporal | At the end of each season |check used quota by local farmer |
|E07 | Local Farmer saved quota | Temporal | At the end of each season |check used quota by local farmer |
|E08 | Water passing on plots | Temporal | During every turn (maybe every hour not specified) |skip wet plot |
|E09 | Dry month | State | total seasonal water / total available water of the season is reduced due to dry month |apply ministry policy |
|E10 | Internet Outage | State | Telecom service / application is offline so online booking is unavailable | allow farmers to book through office |
|E11 | water demand > Supply | State | water demand / total available water of the season is limited | apply ministry policy |
|E12 | Smart Gate mulfunctioning | State | Gate / water isn't delivered or flows in unexpected times | report gate corruption |
|E13 | Sensor failure | State | sensor / system gets no readings or wrong ones so skip suggestions are false | report sensor failure |

### Notes

1. E11's & E03's UCs could be merged to one use case
2. E09's UC could be merged too with E11's & E03's if we assumed that we would know at the start of the season that a dry month will occur
3. update farmer details triggered UC for E02 might be ignored because the significant point is recalculating new quota for his change rather than updating the new plot in the info