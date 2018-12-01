# PK_MUV

This page contains the description of the kit.

## Intro

## Application
The PK_MUV is a WiFi module (esp8266) with NFC reader (RC522).
The PK_MUV kit is programmed to read Tag_MUV. When the user operates the TAG_MUV on PK_MUV kit, the check-in information are sent to the server and they are:
* Tag_MUV UID to identify the user
* PK_MUV ID to identify the location of the kit.
To have access to the key, please contact XXX.

## Instructions
### Connect the PK_MUV to the local WiFi
Turn on the PK_MUV (ON/OFF switch). If the kit is not connected to the WiFi, the Config Led is on/blue, the kit is ready to be connected and it create a network named MUV.
At this point you need a smartphone/tablet or computer, join the network MUV.
<p align="center"><img src="images/config_0.png"></p>


Automatically on the device you are using (smartphone/tablet/computer) the configuration window will pop-up.
<p align="center"><img src="images/config_1.png"></p>
If the window doesn't appear, open a browser and go to the address: http://192.168.4.1/.
<p align="center"><img src="images/config_3.png"></p>




### Modes and Routines
* configuration mode
* sleep mode
* start-up routine
* tag routine
* check routine

#### Configuration Mode
The kit is in configuration mode when it is not connected to the Local WiFi. In configuration mode the Config Led is blue and blinks.
You can enter in configuration mode with the following steps: keep pushed the Config switch and reset the kit. Hold the Config switch until the Config Led blinks blue and you can connect the PK_MUV to the local Wifi, see previous section "Connect the PK_MUV to the local WiFi".

#### Sleep Mode
If the kit has been successfully configured, it enters in sleep mode.
The Tag Led and the Config Led are off and the NFC reader is ready to accept tags. The WiFi module is off.

#### Tag Routine
When the reader get a tag, the Tag Led blinks and the light colour sequence code is:
* green - aqua - green - aqua: the tag payload has been successfully sent to the server, see payload section in

####

## Battery

## MUV Tags

## Troubleshooting
