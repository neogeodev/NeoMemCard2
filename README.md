# NeoMemCard2
Open Hardware NeoGeo memory card

# Files

* neomemcard2_ss : With "NeoGeo" logo silkscreen
* neomemcard2_no_ss : Without "NeoGeo" logo silkscreen

# Operation
The switch allows to select one of the 16kB banks. The NeoGeo system ROM can only handle max. 16kB memory cards.
The 32kB FRAM chip can be replaced by older and maybe cheaper Ramtron 8kB FM16W08's, no need for the switch and pull-up resistor R1 in that case.

The LED turns on as soon as the card is powered. When a game is saved, the LED turns off briefly.

# BOM
| PCB Ref | Manufacturer/Desc       | Mouser Ref           |
|---------|-------------------------|----------------------|
| C1      | 1206 100nF MLCC         | Any                  |
| C2      | 1206 22nF MLCC          | Any                  |
| CONN    | Hirose memcard connector| 798-IC1HA68RD127SH51 |
| D1      | 1206 monochrome LED     | Any                  |
| D2      | BAS16GWX diode          | 841-BAS16GWX         |
| R1      | 1206 4.7k resistor      | Any                  |
| R2      | 1206 8.2M resistor      | Any                  |
| R3      | 1206 ~390ohm resistor   | Any                  |
| SW1     | C&K SPDT slide switch   | 611-SK12C0405SG1.5RT |
| U1      | 32kBytes parallel FRAM  | 877-FM28V020-SG      |
| U2      | 74LVC2G04 dual inverter | 771-74LVC2G14GWQ100H |

R3's value can be changed to adjust LED brightness.