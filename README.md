## Bootloaders for the PX4 boards ##

[![Build Status](https://travis-ci.org/PX4/Bootloader.svg?branch=master)](https://travis-ci.org/PX4/Bootloader)

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/PX4/Firmware?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

* Build instructions: [Documentation](http://px4.io/dev/px4_bootloader)
*   License: GPL for infastructure, BSD for core bootloader (see LICENSE.md)
*   Mailing list: [Google Groups](http://groups.google.com/group/px4users)

## New features ##

*  mix the SD_upload method into the original BOOTLOADER ,if there is a file which named 'fw.bin',this program will upload this firmware automaticlly ,and change the name into 'old' after uploading;if there is a file which named 'old' ,this program will delete it ;

*  add the backup feature,  before erase the chip the program will backup the firmware and named 'backup.bin'.if fail to upload or interrupt during the uploading ,the 'backup.bin' will write into the chip automaticlly next restart ,and change the file name into 'old'.
