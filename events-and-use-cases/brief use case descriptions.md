# Brief use cases descriptions

| **UC ID** | **UC name** | **Brief UC Description** | **Actors** | **Triggering Events** |
|:----:|:----:|:----:|:---:|:---:|
|U01 | Register crops | The farmer registers the crops planned for each of their plots. | Local farmer | Local Farmer wants to register his corps  |
|U02 | Update farmer details | The system updates farmer contact details when farmer changes them. | Local farmer | Local Farmer changes his contact details  |
|U03| Adjust farmer plots | The farmer changes or drops a plot, and the system updates the plot details. |  Local farmer | Local Farmer changes or drops plot |
|U04| Assign turns to local farmers | The scheduler assigns each farmer irrigation turns depending on preferences and quota |  Association head / Local farmer | Turns are assigned to local farmers |
|U05| Give total available seasonal water | The Water Authority sends the total water available for the season, which system compares with demand |  Water Authority | Water authority gives total seasonal water |
|U06| Book irrigation turn | The farmer chooses their preferred slots and which slots they do not want. |  Local farmer | Local Farmer wants to choose slot |
|U07| Calculate season quota | the system calculates the seasonal quota for the farmers  | local farmer  | farmer registered crops |
|U08| Notify local farmers their seasonal quota | the farmers are informed about their seasonal water quota |  Local Farmer | start of new season |
|U09| Earn priority next season | farmers that save quota earn priority next season | local farmer | Local Farmer saved quota |
|U10| Pay fee | farmers that exceed quota pay a fee | tbd | Local Farmer exceeds quota / Local Farmer saved quota |
|U11| Skip wet plot | the system suggests to skip a turn based on how wet the soil is | Smart Sensors / Local Farmer | Water passing on plots |
|U12| Negotiate with local farmer | association head negotiates with farmers to move to allow everyone to have an appropriate schedule | Association Head / Local farmer | Schedule conflict |
|U13| Apply ministry policy | ministry chooses a policy to apply when demand is higher than supply | Water Authority / Ministry | Dry month / water demand > Supply |
|U14| Allow farmers to book through office | farmers can book through office if they do not have internet connection | Local Farmer | Internet Outage |
|U15| Report gate malfunction | system alerts Canal Engineer of malfunctions | Canal Engineer / Gatekeeper | Smart Gate mulfunction |
|U16| Open and close automatically | the smart gates open and close automatically at the start and end of turns | Smart Gate Vendor | start and end of turns |
|U17| Report soil moisture | every hour the sensor reports the soil moisture | IoT Sensor  | Every hour |
