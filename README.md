# Arbotix driver

This is a fork of the ArbotiX-M hardware and library files which makes it compatible Arduino 1.6+

Here is the documentation for the original files:
http://learn.trossenrobotics.com/index.php/getting-started-with-the-arbotix/7-arbotix-quick-start-guide

To use this repo and subsequently your Arbotix-M robot controller for
a project, check it out into a subdirectory of hardware under your
sketchbook directory.

Eg: `<your sketchbook directory>/hardware/<arbotix. this repo>`

libraries are included. example sketches are not. 


### changes

 - moved all directories to be under avr/
 - suppressed errors about poisoned "SIG_USART1_RECV" by adding `#define __AVR_LIBC_DEPRECATED_ENABLE__ 1` to Arduino.h
 - copied platform.txt from arduino/avr over
 - added build.tool and upload.tool to boards.txt
 - moved libraries over to a subdirectory under hardware
