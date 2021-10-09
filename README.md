# goodweDT2mqtt
Polls GoodWE-DT Inverter and publishes Values to mqtt.

## SetUp:
Edit goodwe.js and 
* change mqclient-var to your MQTT-Server
* change HOST to your GoodWE-DT-Inverter WLAN-Stick

## Operation:
* Run in f.ex. in pm2 or in tmux
* Polls Data from Inverter every 15seconds (changeable with var `interval` in Script)

Disclaimer:
Only proof-of-concept.
Some weird things occured here, when developing this. For example the inverter exposes a complete Dataset with the correct CRC, but the Values are bullshit. Tried to catch those things in the Script.
