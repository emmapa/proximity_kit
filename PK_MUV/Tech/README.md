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

BLOCK DIAGRAM

The boards are made using the small milling machine Roland Modela MDX-20, each pcbs require two jobs: mill the trace and cut/drill the boards, in the folder digital files you find the png machinable files.
Tools used:
- one side copper plate, FR1
- to mill the traces: endmill, 0,4mm diameter
- to cut and drill: endmill, 1/64 inch diameter

The files used on the machine are in the folder [Machinable files](https://github.com/emmapa/proximity_kit/tree/master/PK_MUV/Tech/Machinable%20files).<br>
The original Eagle files are in the [Eagle files](https://github.com/emmapa/proximity_kit/tree/master/PK_MUV/Tech/Eagle%20files).

#### PK_MUV pcb

| top view  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_bottom_view.png"></p> |

**note**: the red traces are jumper wires placed on the top layer

#### PK_MUV_L1 pcb

| top view  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_L1_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_L1_bottom_view.png"></p> |

#### PK_MUV_L2 pcb

| top view  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_L2_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_L2_bottom_view.png"></p> |

#### PK_MUV_sw pcb

| top View  | bottom view |
| ------------- | ------------- |
| <p align="center"><img src="images/PK_MUV_sw_top_view.png"></p>  | <p align="center"><img src="images/PK_MUV_sw_bottom_view.png"></p> |

#### Battery cable

#### Assembly note
