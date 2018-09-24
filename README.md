
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/front.jpg">
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/back.jpg">
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/front-detail.jpg">



## Overview
* Designed for soundcard balanced inputs
* Designed to complement [headless audio measurement workstation](https://github.com/pavhofman/measurement-station)
* Can be switched to unbalanced mode (single-ended SE)

## Speaker Load
* Load resistors - combination of 4R and 8R 100W resistors (ebay)
* Inexpensive CPU heatsinks with fans
* Fans powered by the measurement PC

## Ranges
Ranges (voltages for ESI Juli):
  1. 1:1 (20Vmax balanced / 10Vmax SE) - divider 2 x 75R
  2. 1:3 (60Vmax balanced / 30Vmax SE) - divider 2 x (75R + 150R)
  3. 1:6 (120Vmax balanced - not supported/60Vmax SE) - divider 2 x (75R + 375R)
* Divider resistors 2W: 20V at (75R + 75R) -> 1.3W per each resistor
* Ground lift for balanced outputs

## Oscilloscope Output
* Each input line is connected to individual BNC connector for oscilloscope
* Ground lift for scope BNCs


## Soundcard Inputs Protection
* Serial output resistors 680R
* Soundcard hot/cold input protection by two internal voltage sources (-12V, +12V)
* Protection diodes - dual low-leakage diodes BAV199
* Both sets of protection batteries checked by built-in voltmeter.



* Designed to fit FS Futro >=S450 case

The adapter in action:

<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/adapter-pc.jpg">
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/adapter-pc-detail.jpg">


## Construction
* Wired, no PCB
* SMD protection diodes soldered to small universal PCBs placed directly onto TSR sockets

<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/inside-back.jpg">
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/inside-front.jpg">

## Load-Resistors Switch
* 3D-printed, designed for regular 32mm rocker switches
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/switch-front.jpg">
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/switch-back.jpg">

Position 2.7ohm - both resistors paralelly
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/switch-2.7.jpg">

Position 4ohm
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/switch-4.jpg">

Position 8ohm
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/switch-8.jpg">


## Measurements
For comparison ESI Juli in virtual balanced inputs mode with L+R jacks shorted

<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/virt-bal-shorted-inputs.png">

Connected adapter, no input signal, virtual balanced inputs. Notice only minor increase in 50Hz noise, overall noise level unchanged.

<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/virt-bal-adapter-no-input.png">

Connected adapter, no input signal, native balanced inputs of ESI.
<img src="https://github.com/pavhofman/speaker-adapter/raw/master/images/native-bal-adapter-no-input.png">

## Git repository
* All Fusion 360, STL, front panel images

## Conclusion
The adapter does not induce any increase in noise of the measurement setup.
