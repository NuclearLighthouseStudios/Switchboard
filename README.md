# Switchboard

This repository contains the KiCAD project files for the Switchboard guitar pedal IO PCB,
designed to be used with my FX Box guitar pedal enclosure or as a handy interface board when breadboarding new effects.

It contains power filtering, input and output jacks, true bypass switching, a status LED and an optional LTC1044 voltage inverter to generate a -9V rail.  
Components numbered in the 10x rage are specific to the voltage inverter and can be left out if it's not needed.

If you just want the Gerber files or a PDF of the schematic check out the releases tab for downloads.

This PCB should be easily manufacturable with most online PCB houses by just uploading the gerber files.

The PCB and enclosure were designed to fit Neutrik NMJ4HCD2 jacks but most jacks that fit the footprint should be fine. Just make sure they have pins instead of lugs and use a ferrule for mounting instead of a nut.

The pin header should be a precision ground one since they're usually lower profile and taller headers might prevent the boards from fitting correctly.
Make sure yours are less than 7.5mm tall.

Check out the accompanying 3D printable enclosure on Thingiverse: https://www.thingiverse.com/thing:4212939

## BOM

*All parts in the 10x range are optional and only for pedals that need a -9V supply.*

| Reference | Quantity | Value   | Description                                  |
| :-------- | -------: | ------: | :------------------------------------------- |
| C1 C103   | 2        | 100n    | Generic ceramic capacitor                    |
| C102      | 1        | 47µ     | Electrolytic capacitor, 16V                  |
| C101 C104 | 2        | 10µ     | Electrolytic capacitor, 16V                  |
| C2        | 1        | 100µ    | Electrolytic capacitor, 16V                  |
| D1        | 1        | LED     | 5mm LED                                      |
|           | 1        |         | 19mm LED standoff for D1                     |
| J4        | 1        |         | Pin Socket, 6 pins, 2.54mm spacing           |
| J3 J5     | 2        |         | Neutrik NMJ4HCD2 Jack                        |
| R1 R101   | 2        | 100     | Metal film resistor 1%, DIN 0207             |
| R2        | 1        | 10k     | Metal film resistor 1%, DIN 0207             |
| SW1       | 1        |         | 3PDT Footswitch                              |
| U101      | 1        | LTC1044 | LTC1044 Switched-Capacitor Voltage Converter |
