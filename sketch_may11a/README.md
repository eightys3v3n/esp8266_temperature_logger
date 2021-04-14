ESP8266 Temperature Logger

# What it does
Runs on an ESP8266 Arduino device, posts the temperature of a DS18B20 sensor to an MQTT server utilizing 2.4GHz WiFi every defined interval.  

# Usage
To configure, change the MQTT_SERVER, MQTT_USER, MQTT_PASS, SSID, PASSWORD defines in the source file.
Compile and send to ESP8266 utilizing Arduino IDE.  

# More
Lasts 2 days on a 5,000mAh power bank in my testing. No powersaving methods utilized, its just on the WiFi the whole time.  
On the ESP8266 board I have, pin 5 in the code is labelled as D1 on the board.  
DS18B20 sensor is also listed as 18B20, 18S20, TO-92, on AliExpress.  
There are other settings to be changed such as the post rate, device ID, and MQTT topic.  
Based on https://www.instructables.com/Remote-Temperature-Monitoring-Using-MQTT-and-ESP82/  
