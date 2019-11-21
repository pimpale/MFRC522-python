# Added Ultralight Support in this fork
Supports NTAG213, NTAG214, NTAG215, NTAG216, and other Ultralight RFIDs

Reading is the same as normal `MFRC522_Read`, but to write use the `MFRC_WriteUltralight`, with a 4 byte long data. This will write to one page. You don't need to authenticate when writing. Runs only with python3, make sure to use it. 

MFRC522-python
==============
A small class to interface with the NFC reader Module MFRC522 on the Raspberry Pi.
This is a Python port of the example code for the NFC module MF522-AN.

**Important notice:** This library has not being actively updated in almost four years.
It might not work as intended on more recent Raspberry Pi devices. You might want to 
take a look to the open pull-requests and forks to see other implementations and bug-fixes.

## Requirements
This code requires you to have SPI-Py installed from the following repository:
https://github.com/lthiery/SPI-Py

## Examples
This repository includes a couple of examples showing how to read, write, and dump data from a chip. They are thoroughly commented, and should be easy to understand.

## Pins
You can use [this](http://i.imgur.com/y7Fnvhq.png) image for reference.

| Name | Pin # | Pin name   |
|:------:|:-------:|:------------:|
| SDA  | 24    | GPIO8      |
| SCK  | 23    | GPIO11     |
| MOSI | 19    | GPIO10     |
| MISO | 21    | GPIO9      |
| IRQ  | None  | None       |
| GND  | Any   | Any Ground |
| RST  | 22    | GPIO25     |
| 3.3V | 1     | 3V3        |

## Usage
Import the class by importing MFRC522 in the top of your script. For more info see the examples.

## License
This code and examples are licensed under the GNU Lesser General Public License 3.0.
