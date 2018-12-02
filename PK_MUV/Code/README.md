 <FS.h>                   // Make sure ESP library 2.1.0 or higher is installed
 <ESP8266WiFi.h>          //https://github.com/esp8266/Arduino
 <DNSServer.h>
 <ESP8266WebServer.h>
 <WiFiManager.h>          //https://github.com/tzapu/WiFiManager
 <ArduinoJson.h>          //https://github.com/bblanchon/ArduinoJson
 <PubSubClient.h>     //https://github.com/knolleary/pubsubclient

#### First upload
In the Arduino sketch define the variable RESET_SETTINGS 1: '#define RESET_SETTINGS 0', to format the System files in the esp8266 and reset previously saved WiFi settings.
Upload the code.

#### Second and further uploads
In the Arduino sketch define the variable RESET_SETTINGS 0: '#define RESET_SETTINGS 0'.

Be sure that the information to connect to the MUV server are correct:

char mqtt_server[41] = "<my_server>\0";<br>
char mqtt_portStr[21] = "<my_port>\0";<br>
char mqtt_username[21] = "<my_username>\0";<br>
char mqtt_password[21] = "<my_password>\0";<br>
char mqtt_topic[21] = "<my_topic>\0";<br>

To get the MUV credential, please [contact](https://github.com/emmapa/proximity_kit/tree/master/PK_MUV#Contacts).
