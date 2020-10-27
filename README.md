# Cmod S7 Root Repository

## Cmod S7-25 Out-of-Box Demo

### Description

This branch contains sources for the Cmod S7-25 Out-of-Box Demo.

This demo is a simple Vivado project using the Cmod S7-25's LEDs, RGB LED, buttons, and USB-UART bridge, written in Verilog.
When programmed onto a Cmod S7, the demo will cycle the board's RGB LED from Blue to Green to Red to off. The other LEDs will light up in sequence.

To use the USB-UART bridge feature of this demo, the Cmod S7 must be connected to a serial terminal (such as Tera Term or PuTTY) on the computer it is connected to over the MicroUSB cable.
Whenever one of the two buttons is pressed, "Button # Pressed!" is sent to the computer using the USB-UART bridge.

For more information on the Cmod S7-25 Out-of-Box Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/demos/oob) on the Digilent Wiki.

For more information on the Cmod S7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Cmod-S7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes               |
| SW        | No                |


This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Cmod-S7-25-OOB

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Cmod S7-25
* Vivado 2020.1 Installation
* Serial Terminal Application, such as Tera Term or PuTTY
* MicroUSB Cable