# inputProtectionShield

The [JTAGULATOR](http://www.grandideastudio.com/portfolio/jtagulator/) took an existing project, the [JTAGENUM](https://github.com/cyphunk/JTAGenum), and reinvented the wheel in a few places. JTAGENUM runs on Arduino, and so this shield provides the Arduino Nano with the exact same hardware capabilities as the JTAGULATOR without the [hefty ($170 for a kit) price tag](https://hackerwarehouse.com/product/jtagulator/).

These hardware capabilities include:

* Input level conversion, including a range from 1.8-5v logic (larger range than JTAGulator)
* Input protection with current limiting and Schottky diode array



## Board

|                                      |                                           |
| ------------------------------------ | ----------------------------------------- |
| ![](https://i.imgur.com/5gnbYKM.png) | ![Imgur](https://i.imgur.com/X8UfBSi.png) |

## Bill Of Materials

* If the HSMS-285R is unavailable, the following parts should work:
  * [NUP4302MR6](http://www.mouser.com/ds/2/308/NUP4302MR6-99757.pdf)
  * [TESD5V0V4UCU6 RFG](www.taiwansemi.com/products/datasheet/TESD5V0V4UCU6_A1705.pdf) (Bought 12 for $4.13, 4x for $1.37)
* MOSFETs: [50pcs BSS138  MOSFET N-CH 50V .22 AMP IN SOT-23 PKG. USA SUPPLIER](http://www.ebay.com/itm/382540619634) ($3.25, $0.065 each, 8x for $0.52)
* Resistors:
  * [Lot of 125 CRCW04021K00FKTD Vishay Chip Resistor 1k Ohm 62.5mW 1/16W 1% 0402 NOS](http://www.ebay.com/itm/201820263322) ($3.99, $0.03192 each, 16x for $0.51)
  * [Lot of 75 RK73H1ELTP1002F KOA Chip Resistor 10k Ohm 100mW 1/10W 1% 0402 NOS](http://www.ebay.com/itm/201683750387) ($5.40, $0.072 each, 8x for $0.57)
* Arduino: [Arduino Nano V3.0 ATmega328 5V Micro-controller CH340E](http://www.ebay.com/itm/391965564336) ($11.50)
* Boards: 6 for $13.40 from OSHPark, $2.23 each

**Total: $16.70** per unit



| **Part**          | **Value**    | **Device**         | **Package** | **Description**                                            |
| ----------------- | ------------ | ------------------ | ----------- | ---------------------------------------------------------- |
| D1-D4 (4x)        | HSMS-285R    | HSMS-285R          | SOT363      | Surface Mount Microwave Schottky Detector Diodes Ring Quad |
| Q1-Q8 (8x)        | BSS138       | MOSFET-NCHANNELSMD | SOT23-3     | BSS138 MOSFET                                              |
| R1-R15, R17 (16x) | 10k          | R-US_R0402         | R0402       | RESISTOR, American symbol                                  |
| R16, R18-R24 (8x) | 1k           | R-US_R0402         | R0402       | RESISTOR, American symbol                                  |
| SV1               |              | FE15-1             | FE15        | FEMALE HEADER                                              |
| SV2               |              | FE15-1             | FE15        | FEMALE HEADER                                              |
| SV3               |              | MA03-1             | MA03-1      | PIN HEADER                                                 |
|                   | ARDUINO NANO | ARDUINO NANO       | PDIP-32     | Arduino Nano                                               |

## Credits

* [JTAGulator Versus JTAGENUM Blog Post](https://p16.praetorian.com/blog/jtagulator-vs-jtagenum-tools-for-identifying-jtag-pins-in-iot-devices) and original board design by Dylan Ayrey. Great work!
* Board layout tweaks (so far just the silkscreening fonts and other aesthetic tweaks) by Erik Gregg