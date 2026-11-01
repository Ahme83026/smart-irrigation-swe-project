# External Events

## 1. Local Farmer changes his contact details

-  **Detailed description:** after already registering in the system, a farmer at some point in time might wanna change his contact details as phone number or acc
  
-  **Responsible actor:** Local Farmer
  
-  **Triggered use cases:** update farmer details

## 2. Local Farmer changes / drops plot

-  **Detailed description:** during a season, a farmer may change his plot to a new location or sell/drop it for reasons as they can't afford maintainning it anymore, found a more appropirate location for them or they dont need it anymore
  
-  **Responsible actor:** Local Farmer
  
-  **Triggered use cases:**
   -  update farmer details
   -  recalculate new quota

## 3. Water authority gives total seasonal water

-  **Detailed description:** at the start of a new season, water authority notifies the total available water
  
-  **Responsible actor:** Water Authority

-  **Triggered use cases:** compare supply and demand

## 4. Local Farmer wants to choose slot

-  **Detailed description:** at the start of a new season, a local farmer wants to choose a slot

- **Responsible actors:** Local Farmer

-  **Triggered use cases:** Book irrigation turn

# Temporal Events

## 1. New Quota Calculation

- **Detailed Description:** At the start of each season, the water needed for specific crops and the quotas are calculated

- **Time:** At the start of a new season

- **Triggered use cases:** calculate season quota

## 2. Local Farmer exceeds quota

- **Detailed Description:** along the season a local farmer exceeded their given and calculated quota

- **Time:** At the end of each season

- **Triggered use cases:** check used quota by local farmer

## 3. Local Farmer saved quota

- **Detailed Description:** along the season a local farmer saved water by skipping

- **Time:** At the end of each season

- **Triggered use cases:** check used quota by local farmer

## 4. Water passing on plots

- **Detailed Description:** when the smart gates are opened during a turn the water pass on the plots registered in that slot

- **Time:** During every turn (maybe every hour not specified)

- **Triggered use cases:** skip wet plot

# State Events

## 1. Dry month

- **Detailed Description:** a dry month occurred

- **Entitiy state changed:** Season (for now, tbd)

- **State change:** total available water of the season is reduced due to dry month

- **Triggered use cases:** tbd

## 2. Internet Outage

- **Detailed Description:** an outage ocuurred in internet connection

- **Entitiy state changed:** Telecom service

- **State change:** application is offline so online booking is unavailable

- **Triggered use cases:** allow farmers to book through office

## 3. water demand > Supply

- **Detailed Description:** the water demand is more than the supplied amount at the start of a season

- **Entitiy state changed:** Season (for now, tbd)

- **State change:** total available water of the season is limited

- **Triggered use cases:** apply ministry policy

## 4. Smart Gate mulfunctioning

- **Detailed Description:** smart gates don't open properly as they should

- **Entitiy state changed:** Gate

- **State change:** water isn't delivered or flows in unexpected times

- **Triggered use cases:** report gate corruption

## 5. Sensor failure

- **Detailed Description:** 

- **Entitiy state changed:** sensor

- **State change:** system gets no readings or wrong ones so skip suggestions are false

- **Triggered use cases:** report sensor failure

# Notes

1. Although water authority gives seasonal water every season, that doesnt imply that the event is temporal because the Water authority is considered an external actor
   
2. In both Local Farmer exceeds quota and Local Farmer saves quota events, despite the farmer is an external actor the event is temporal because regardless of the farmer exceeding or saving or none the use case is triggered seasonaly to check and apply appropriate procedure not triggered by an external actor









