# Altoids Serial Adapter

**Latest News**

* **DESIGN IN PROGRESS. UNTESTED**

## Introduction

Fed up with having to use multiple USB serial adapters and wiring configurations? Just want to plug in and go. This project was born from a desire for a quick and neat way to interface with various single board homebrew computers (SBCs)- such as the Kim-Uno, Southern Cross and SC131 to name a few. Most USB serial adapters are bare boards, have tiny pin labels and come with different logic voltages and pin out orders. This makes it a fiddle to set up. What power, what logic, mess around switching dupont jumper cables between the correct pins....
With the Altoid Serial Adapter the fiddle is over. You're welcome!

## Credits and thanks

Credits and thanks are worthy of being up front.

* **Lee Hart** for inspiring the look and feel of this project. Please check out his site for some amazing SBCs. https://www.sunrise-ev.com/index.htm
* Tom Van Baak for the brilliant picDIV™ project. Please check out his site for all things clock.
* bborncr for the initial PCB outline and sizing to fit the Altoids tin. https://github.com/bborncr/AltoidsPCB
* FTDI 

## General Aims

* Provide 'plug and play' connections using fixed ribbon cables for the most typical serial pin connection order. I don't want to be crossing wires and tracing wire colours.
* Provide some nice LEDs.
* Switchable power and serial logic voltages.
* Fit it all to look nice and tidy in an Altoids tin.
* For ease, safety and to simplify both design and assembly (and probably cost) use commercially available modules for the power regulation, multiplexing and charging.
* Limit the SMD to ease assembly.

## Bespoke Aims

These are added features that suit more bespoke applications.

* SBCs such as the Kim-Uno and Membership Cards dont always warrant a serial connection as they can be programmed by switches and buttons. Therefore why not provide some onboard battery power.
* With an onboard battery, may as well be able to charge it.
* As we have regulated power we may as well break it out - to be useful for other things.
* Sometimes you may need a signal High or Low? My use is that some SBCs need a High or Low to activate a display. Provide a switch for that, i like switches.
* Ok, the serial adapter IC has an onboard oscillator. It would be a shame to waste that. Wait, the oscillator runs at 2024 speeds, i need something slower for 1980s tech. Use a PIC to divide the clock and provide a breakout for sub 6MHZ clock signals. Might come in handy.
* For the clock, provide breakouts for onboard PIC programming. This then offers more possibilities without having to disassemble the board.

## Final Features

![](https://github.com/Kayto/Altoids_Serial_Adapter/blob/main/images/readme1.jpg)
![](https://github.com/Kayto/Altoids_Serial_Adapter/blob/main/images/readme.jpg)

In no particular order the main features in the final board are as follows.

- Programmable clock breakout using the picDIV™ project.
- Indicator LEDs for the main functions and configurations.
- Onboard Li-ion battery charger.
- Selectable 5V and 3V3 power and logic.
- Seperate Power breakout.
- High and Low signal logic breakout

## Build

Coming Soon.

### REVISION STATUS & ISSUES
**REV 000**
* DRAFT DESIGN IN PRODUCTION. UNTESTED AT THE MOMENT.

## Firmware

Comming soon.
Instructions for the FT232R clock configuration.
Instructions for the picDIV™ project.

## Licenses & acknowledgement
Further to the links in the credit section.

**KiCad Library**

**picDIV™**
http://www.leapsecond.com/pic/
http://www.leapsecond.com/pic/src/readme


