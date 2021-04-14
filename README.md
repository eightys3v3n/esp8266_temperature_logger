ESP8266 Temperature Logger

# What it does
Runs on an ESP8266 Arduino device, posts the temperature of a DS18B20 sensor to an MQTT server utilizing 2.4GHz WiFi every defined interval. Also supports HomeAssistant integration.  

# Usage
To configure, create espurna/code/espurna/config/credentials.h and insert the following into it, changing for your usecase.
```C
#define WEB_USERNAME "admin"
#define ADMIN_PASS "default_password_to_login"

#define WIFI1_SSID "WIFI_NAME"
#define WIFI1_PASS "WIFI_PASSWORD"

#define MQTT_AUTOCONNECT 1
#define MQTT_USER "MQTT Username"
#define MQTT_PASS "MQTT Password"
#define MQTT_PORT 1883
#define MQTT_SERVER "MQTT server url"
#define MQTT_QOS 2
```  
Compile by navigating into espurna/code and running build.sh.  
Connect to the device using the web interface, in HASS enable discovery and in MQTT enable.  
