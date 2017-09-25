This is a collection of perl scripts for working with a 3D printer (specifically
the Anycubic Kossel Plus).

The Marlin firmware should be compiled to run at 115200 baud to prevent issues
setting the serial port to the correct (250000) baud rate (Linux really doesn't
like that baud rate, and there is zero reason to run at it anyway).

gcodeserver
====

Monitors a folder (/shared/GCode by default) for .gcode files and prints
them automatically.

level
====

Bed levelling control panel (GTK)

sendgcode
====

Script to send a .gcode file to the printer

Prerequisites
=============

```
apt-get install libdevice-serialport-perl libgtk2-perl
```


