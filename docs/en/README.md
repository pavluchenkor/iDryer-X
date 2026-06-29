# iDryer X

The X series has moved to a new platform. Learn more in the iDryerControllerV2 section.

Support for the current platform continues.

A universal filament drying solution for 3D printing enthusiasts.
You can build it using affordable and accessible parts - for example, an old heater, a spare fan and heatsink, a storage box, and any insulation material. The list of parts is limited only by your imagination.

DIY builds are available in the DIY section.

There is also a KIT version that includes everything you need: pre-machined enclosure parts, electronics, metal base parts, spool holders, a heater, and a fan.
Assembly instructions for the KIT version can be found in the iDryer v3 section.

## Dryer Advantages

<div class="grid cards" markdown>

-   :material-sun-thermometer-outline:{ .lg .middle }__Heating up to 110°C__

    ---

    Set your desired temperature via menu and the device will automatically maintain it throughout the drying process. Capable of drying any filament available on the market.

-   :material-weather-pouring:{ .lg .middle }  __Humidity Control__

    ---

    Automatic heating when the humidity exceeds the set threshold.

-   :material-scale:{ .lg .middle } __Spool Weight Monitoring__

    ---

    Measures the spool weight and alerts when filament runs out.

-   :material-home-lightning-bolt:{ .lg .middle } __Energy Efficiency__

    ---

    iDryer is highly energy-efficient, allowing continuous 24/7 operation without breaking your budget.

-   :material-hand-coin-outline:{ .lg .middle } __Low Cost__

    ---

    iDryer is a cost-effective DIY solution. All components are affordable and printable on a 3D printer.

-   :material-bitcoin:{ .lg .middle } __Build It Yourself__

    ---

    A dryer for 4 spools with built-in weight tracking can be assembled for under $80-100, making iDryer a unique solution in its class.

</div>

## Features

### Drying

* Set drying temperature and duration
* Precise temperature maintenance
* Display of current humidity
* Automatic switch to storage mode

### Storage

* Maintain target humidity level
* Automatic heater and fan control based on humidity
* Unlimited storage duration

### Presets

* Save frequently used filament profiles
* Set temperature and time for each preset

### General Functionality

* PID control of heater power
* Safe heating for all filament types
* Precise temperature regulation
* Humidity monitoring in the chamber

### Energy Efficiency

* Drying mode \~ 40W/hour
* Storage mode \~ 20W/hour
* Standby mode \~ 3W/hour

### Chamber Ventilation

* Servo-controlled air damper
* Set "open" and "close" times for air exchange

## Firmware

[The firmware file](https://github.com/pavluchenkor/iDryerController/blob/master/src/Configuration.h) contains all possible configurations.

### Arduino Bootloader Firmware

!!! warning "Not Recommended"

* No watchdog timer
* No servo support
* No additional PWM channel
* No spool weight monitoring
* No longer actively developed

### Minicore Core Firmware

* Watchdog timer enabled - auto reset on failure
* Servo support
* Additional PWM channel
* Extended menu and functionality
* Improved firmware safety

> Arduino core firmware can be used on early versions but is not recommended. It's better to buy a programmer, reflash the bootloader, and use the safer firmware.

!!! note annotate "Project files on GitHub"

```
[iDryer v1 prototype](https://github.com/pavluchenkor/iDryer) - a minimal, affordable prototype of the dryer

[iDryer v3](https://github.com/pavluchenkor/iDryerController) - current open-source version with firmware and full design files
```

<!-- [![Telegram](https://img.shields.io/badge/Telegram-Join%20Group-blue)](https://t.me/iDryer)  [![YouTube](https://img.shields.io/badge/YouTube-Watch%20video-red)](https://www.youtube.com/@iDryerProject) [![Rutube](https://img.shields.io/badge/Rutube-Watch%20video-blue)](https://rutube.ru/channel/34401569/) -->
