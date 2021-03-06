# Parts
The PK_MUV kit is a portable device made of the following parts and features:

* Mcu/WiFi: Adafruit Feather HUZZAH esp8266 board
* NFC Reader: RC522 NFC reader
* Visual feedback: 3 WS1282 LEDs
* Audio feedback: buzzer
* Power switch
* Reset button
* Configuration button
* Indicator RGB Led for battery status
* Indicator RGB Led for configuration mode
* Indicator RGB Led for feedback
* Power supply: rechargeable battery or micro USB cable
* 6 mounting holes

The PK_MUV uses two off-the-shelf boards, the Adafruit Feather HUZZAH esp8266 and the NFC reader RC522, and four boards made in the fablab, the PK_MUV pcb, the PK_MUV_L1 pcb, the PK_MUV_L2 pcb and the PK_MUV_sw pcb.

<p align="center"><img src="images/block_diagram.png"></p>

The boards are made using the small milling machine Roland Modela MDX-20, each pcbs require two jobs: mill the trace and cut/drill the boards, in the folder digital files you find the png machinable files.
Tools used:
- one side copper plate, FR1
- to mill the traces: endmill, 0,4mm diameter
- to cut and drill: endmill, 1/64 inch diameter

The files used on the machine are in the folder [Machinable files](https://github.com/emmapa/proximity_kit/tree/master/PK_MUV/Tech/Machinable%20files).<br>
The original Eagle files are in the [Eagle files](https://github.com/emmapa/proximity_kit/tree/master/PK_MUV/Tech/Eagle%20files).

In Fablab Amsterdam the software to generate the rml file and send it to the machine is Fabmodules. It is highly recommended to use the last version of Fabmodules, aka mods http://mods.cba.mit.edu/; previous versions of fabmodules, still work but double check the output of the software before to send the job to the machine, in some cases the path is not well calculated.

In the image below you find the setting to envrage the traces and to drill holes/cut the board.
<img src="images/config_traces.png" width="500"><br>
<img src="images/config_outlines.png" width="500">

Note: when you mill the outlines, you will need to trick the fabmodules!! Some holes are two smalls to be identified with a diameter tool of 1/64inch (0.79248mm) so you can set the diameter tool to 0.78mm and all the holes will be milled; yes, you loos some copper on the pad but it is still enough to solder vias and components.

#### PK_MUV pcb

| top view  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_bottom_view.png"></p> |
| All the header are THT, pitch 2.54mm. <br> JP_LEDS: 1x3 female header, THT <br> JP_BUZ: holes for piezo<br> JP_SW: 2x2 male header<br> Feather header 1: 1x16 female header<br> Feather header 2: 1x16 female header<br> JP_LED_TAG: 1x4 female header<br> JP_NFC: 1x8 female header <br> | All the resistors are smd 1206. <br>R1: 1M Ohm<br> R2: 220k Ohm<br> R3: 0 Ohm<br> R4: 0 Ohm<br> R5: 10k Ohm<br> R6: 470 Ohm <br> R7: 0 Ohm<br>|
| <p align="center"><img src="images/PK_MUV_top_clean.jpg"></p>  | <p align="center"><img src="images/PK_MUV_bottom_clean.jpg"></p>|
|<p align="center"><img src="images/PK_MUV_top_stuffed.jpg"></p>| <p align="center"><img src="images/PK_MUV_bottom_stuffed.jpg"></p>

**note**: the red traces are jumper wires placed on the top layer

#### PK_MUV_L1 pcb

| top view  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_L1_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_L1_bottom_view.png"></p> |
| The header is THT, pitch 2.54mm. <br> JP1: 1x04 male header 90° | Capacitors is smd 1206. <br>C1: 0.1uF <br> U1: WS2812B Led|
| <p align="center"><img src="images/PK_MUV_L1_top_clean.jpg"></p>  | <p align="center"><img src="images/PK_MUV_L1_bottom_clean.jpg"></p>|
| <p align="center"><img src="images/PK_MUV_L1_top_stuffed.jpg"></p>  | <p align="center"><img src="images/PK_MUV_L1_bottom_stuffed.jpg"></p>|


#### PK_MUV_L2 pcb

| top view  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_L2_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_L2_bottom_view.png"></p> |
| The header is THT, pitch 2.54mm. <br> JP1: 1x03 male header 90°   | Resistors and capacitors are smd 1206. <br>C1=C2: 0.1uF <br> U1=U2: WS2812B Led |
| <p align="center"><img src="images/PK_MUV_L2_top_clean.jpg"></p>  | <p align="center"><img src="images/PK_MUV_L2_bottom_clean.jpg"></p>|
| <p align="center"><img src="images/PK_MUV_L2_top_stuffed.jpg"></p>  | <p align="center"><img src="images/PK_MUV_L2_bottom_stuffed.jpg"></p>|


#### PK_MUV_sw pcb

| top View  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_sw_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_sw_bottom_view.png"></p> |
| sw1 = sw2: Tactile Switch THT | The header is smd, pitch 2.54mm <br> JP1: 2x2 male header<br> |
| <p align="center"><img src="images/PK_MUV_sw_top_clean.jpg"></p>  | <p align="center"><img src="images/PK_MUV_sw_bottom_clean.jpg"></p>|
|<p align="center"><img src="images/PK_MUV_sw_top_stuffed.jpg"></p>| <p align="center"><img src="images/PK_MUV_sw_bottom_stuffed.jpg"></p> |

#### Battery cable

#### Assembly note

#### BOM notes
Many items in the BOM can be bought only in minimum amount, when you actually are going to use one or two component. The total cost is therefore expressed as:
* total purchase: the cost of the purchase, buying the minimum amount per items
* cost of 1 kit: considering the cost of only the component used in the kit.

for example: if you buy the "feather header 1" from Farnell, you have to buy 10 components even if you are going to use only one. In the purchase cost the item "feather header 1" is 12€ but in the single cost of one kit, the item value is 1,2€.
