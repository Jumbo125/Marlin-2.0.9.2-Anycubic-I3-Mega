# Marlin-2.0.9.2-Anycubic-I3-Mega
## Marlin 3D Printer Firmware

![GitHub](https://img.shields.io/github/license/marlinfirmware/marlin.svg)
![GitHub contributors](https://img.shields.io/github/contributors/marlinfirmware/marlin.svg)
![GitHub Release Date](https://img.shields.io/github/release-date/marlinfirmware/marlin.svg)
[![Build Status](https://github.com/MarlinFirmware/Marlin/workflows/CI/badge.svg?branch=bugfix-2.0.x)](https://github.com/MarlinFirmware/Marlin/actions)

<img align="right" width=175 src="buildroot/share/pixmaps/logo/marlin-250.png" />

 ### !IMPORTANT! 
 I use the marlin software and edit some code parts, to pass it for my Anycubic.
 It isn't my own work, so i thank the marlin developers for this great work!
 
 I need to do some changes. These are in configuration.h, configuration_adv.h, pins.h, pins_TRIGORILLA_14, pause.ccp and anycubic_i3mega_lcd.cpp.
 
 
 ### Fixes:
 #### 1. Missing Dual Z-Stepper
 1.1 Set Z2 pins from E1 pins. (Only one Extruder)
 1.2 Change default pins in pins.h file
 1.3 DISABLE Software Z-Endstop
 1.4 Invert Z-Endstop
 
 #### 2. MEsh Bed Leveling
 2.1 Enable Auto Biliniear Leveling with manual probe (without any sensor)
 2.2 Change gcode behinde start leveling button in special menu
 2.3 Disable some code parts in pause.cpp to disable the choice menu between purge more and continue
 
 #### 3. Park advance
 3.1 Disable show_lcd_ menu after reheat noozle
 3.2 Show Continue button after reheat noozle
 
 So. i hope you have fun
 
 The firmware is in the directory source code/pio/build/mega2650/*.hex
 
 for e.g. my bed:
 <img src="https://github.com/Jumbo125/Marlin-2.0.9.2-Anycubic-I3-Mega/blob/main/mbl_view.JPG" alt="my_bed">
 
