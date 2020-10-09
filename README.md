# MisonoWorks Volt

![Preview image](https://i.imgur.com/2kWvzd2.jpg)

A pocket-sized Sound Voltex controller, with WS2812B underglow.
Uses keyboard switches, EC11 encoders and an HRO TYPE-C-31-M-12 USB-C receptacle.

This repository is covered by a GNU General Public License v3.0. You may reproduce these controllers commercially with attribution. For any inquiries, please contact me at misonoworks@gmail.com

## ASSEMBLY INSTRUCTIONS
1) Download the files and put them into an easy-to-reach spot
2) Go to jlcpcb.com and create an account
3) Click the big blue "QUOTE NOW" button and upload pocket voltex.zip
4) Check all of your settings. If you are using their SMD service, you can only use green soldermask.
5) Repeat this process for plate.zip if you want to use 3pin switches
If you are going to use JLCPCB's SMD assembly service, continue to the JLCPCB SMD SERVICE INSTRUCTIONS section

## JLCPCB SMD SERVICE INSTRUCTIONS
1) After completing Step 4 of Assembly Instructions, scroll down and click the SMT Assembly button
2) Assemble the BOTTOM of the PCB and select how many assembled units you want
3) Upload pocket voltex bom jlcpcb.csv to the BOM field
4) Upload pocket voltex pos file jlcpcb.csv to the centroid file field
5) Continue, select your parts from the fields provided. If you want to use exactly what I used for everything, reference the parts list below.
6) Use the gerber viewer to check that everything is OK
7) Order, and done!
Note that, regardless if you opt to use the SMD assembly service, you will still need to solder the USB C port as JLCPCB does not have them stocked.

## SMD SOLDERING TOOLS LIST AND INSTRUCTIONS
### Required tools:
Soldering iron
Solder braid
Solder
Tweezers
### Useful tools: 
Magnifying glass
Solder paste
Low-diameter heat gun nozzle and heat gun
Variable temperature soldering iron

Follow this guide to learn how to solder SMD parts.
https://youtu.be/VxMV6wGS3NY

### SOLDERING THE USB C PORT
This might seem daunting at first, but it's actually really, really easy.
1) Fix your USB C connector to the pads by putting a small blob of solder on them
2) Solder the through-hole connections to ensure it doesn't move or rip off
3) Cover all of the connections with one big blob of solder. 
4) Take your solder wick and thoroughly suck up all shorts between the leads.
5) Make sure you get into the nooks and crannies so you decrease the risk of shorting your MCU or fuse.p
6) Done!
I'll upload some photos of this when I get some new PCBs in

## PARTS LIST
USB C Connector (REQUIRED FOR BOTH SMD ASSEMBLY USERS AND HAND-ASSEMBLERS) - https://lcsc.com/product-detail/USB-Type-C_Korean-Hroparts-Elec-TYPE-C-31-M-12_C165948.html

ATMEGA32U4 - https://lcsc.com/product-detail/ATMEL-AVR_Microchip-Tech-ATMEGA32U4-AU_C44854.html

Crystal - https://lcsc.com/product-detail/SMD-Crystal-Resonators_Yangxing-Tech-X322516MLB4SI_C13738.html

Rotary Enccoders (any EC11 clone encoder will work) - https://www.digikey.com/en/products/detail/PEC11L-4020F-N0020/PEC11L-4020F-N0020-ND/4699164?utm_medium=email&utm_source=oce&utm_campaign=3480_OCE20RT&utm_content=productdetail_US&utm_cid=1463922&so=65741090&mkt_tok=eyJpIjoiWVdaaVlUa3hOVEkwWVRRMCIsInQiOiJzQWczcjlXa1hBbkZrVDlXa01PenZTQVZmWThYYVYxenh4MktSbnhnbVAxblp2VGdvUlhGY2FGOXVYREprWmR1aDZQaW1KXC8zSUdWa1FtaGJ3MXV6MkNTcFR3RUltN21yYWV4NUJydVVlcENqUFpUTnF6UkxtMnl4WlVSMjk3bGsifQ%3D%3D

Reset Switch - https://lcsc.com/product-detail/Tactile-Switches_XKB-Connectivity-TS-1187A-B-A-B_C318884.html

500mA Fuse - https://lcsc.com/product-detail/PTC-Resettable-Fuses_Littelfuse-1206L050-15YR_C151162.html

WS2812B - https://lcsc.com/product-detail/Light-Emitting-Diodes-LED_Worldsemi-WS2812B-B_C114586.html

100nF Capacitor (for WS2812B) - https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_YAGEO-CC0805KRX7R9BB104_C49678.html

10kΩ Pull-Down Resistor (FOR MCU) - https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_UNI-ROYAL-Uniroyal-Elec-0805W8F1002T5E_C17414.html

22Ω Data Lead Resistor (FOR USB) - https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_UNI-ROYAL-Uniroyal-Elec-0805W8F220JT5E_C17561.html

5.1k Pull-Down Resistor (FOR USB) - https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_UNI-ROYAL-Uniroyal-Elec-0805W8F5101T5E_C27834.html

1nF Decoupling Capacitor (FOR MCU) - https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Samsung-Electro-Mechanics-CL21B105KBFNNNE_C28323.html

220 Resistor (FOR THT LEDS) - https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_UNI-ROYAL-Uniroyal-Elec-0805W8F2200T5E_C17557.html

22pF Decoupling Capacitor (FOR CRYSTAL) - https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Samsung-Electro-Mechanics-CL21C220JBANNNC_C1804.html

Keyboard switches (make sure to pick MX COMPATIBLE switches!) - https://novelkeys.xyz/collections/switches

BT Keycaps - https://pimpmykeyboard.com/dsa-1-5-space-pack-of-4/

FX Keycaps - https://pimpmykeyboard.com/dsa-2-space-pack-of-4/

Start Keycaps - https://pimpmykeyboard.com/dsa-1-space-pack-of-10/

Knobs (Aliexpress, cheap, matte color with no dial indicator) - https://www.aliexpress.com/item/32912465745.html?spm=a2g0s.9042311.0.0.f83b4c4dPglQ28

Knobs (Amazon, fast, expensive, metallic with colored dial indicator) - https://www.amazon.com/gp/product/B07PQ5H6MF/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1
