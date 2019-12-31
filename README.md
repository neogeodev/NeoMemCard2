# NeoMemCard2
Open Hardware NeoGeo memory card

# Files

* neomemcard2_ss : With "NeoGeo" logo silkscreen
* neomemcard2_no_ss : Without "NeoGeo" logo silkscreen

# Operation
The switch allows to select one of the two 16kB banks. The NeoGeo system ROM can only handle max. 16kB memory cards.

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
| U1      | 32kBytes parallel FRAM  | 877-FM18W08-SG       |
| U2      | 74LVC2G04 dual inverter | 771-74LVC2G14GWQ100H |

# Notes
The 74LVC2G04 is in a small package, it may be challenging to solder.

The 32kB FRAM chip can be replaced by older and maybe cheaper Ramtron 8kB FM16W08's, no need for the switch and pull-up resistor R1 in that case.

R3's value can be changed to adjust the LED's brightness.

Use electrical tape or a piece of adhesive vinyl sheet to cover the components. Not doing so may result in their tearing by the plastic ridges inside the console during insertion or removal of the card.

# License and guarantee

In general, if you plan on using **free** and open source files which (as clearly stated by section 16 of the LICENSE file) don't come with any kind of guarantee and even less any kind of contractual service since they're basically **a gift**, please don't be like some dude named Andreas P. and feel entitled to obtain lengthy e-mail assistance and blame me for frying 30€ worth of chips because there was a mistake in the component list and you didn't check it yourself.

Imagine how much of an ass you'd sound like if you expected excuses from your aunt for mixing up salt with pepper in the recipe she gave you for your cake selling stand.
