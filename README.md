# Cmod S7 Root Repository

## Cmod S7-25 Microblaze XADC Demo

### Description

This branch contains sources for the Cmod S7-25 Microblaze XADC Demo.

This project demonstrates how to use the Cmod S7-25's Spartan 7 FPGA's analog-to-digital core (referred to as the XADC) with a Microblaze processor. Vivado is used to build the demo's hardware platform, and Vitis is used to build and deploy a C application.

To use this demo, the Cmod S7 must be connected to a computer over MicroUSB, which must be running a serial terminal (such as Tera Term or PuTTY).

As long as the demo is running, ten times per second, the voltages on each of the Cmod S7-25's DIP header's analog input pins (AIN32 and AIN33) are read and printed to a connected serial terminal. The readings are accurate to two decimal places. To avoid damage to the FPGA, take care not to apply a voltage greater than 3.5 Volts to the analog pins. Any voltages less than 0 Volts or greater than 3.3 Volts are read as those instead.

For more information on the Cmod S7-25 Microblaze XADC Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/demos/xadc) on the Digilent Wiki.

For more information on the Cmod S7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cmod-s7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Cmod-S7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes               |
| SW        | Yes               |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Cmod-S7-25-XADC

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Cmod S7-25
* Vivado and Vitis 2020.1 Installations
* Serial Terminal Emulator (such as Tera Term or PuTTY)
* MicroUSB Cable for programming and USBUART communication
* Circuit to measure (a breadboard is recommended)