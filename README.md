# Touchdesigner Helpers
An open collection of useful tools around Derivative Touchdesigner.


## Components
### Table of contents
* [Beat Pulse](#beat-pulse)
* [Color Picker](#color-picker)
* [DMX Map](#dmx-map)

### Beat Pulse
Outputs a pulse (maximum value of 1) in sync with the global project tempo.

#### Parameters
**Pulse Length** 
*(Value between 0 and 1)*
Determines the fraction of "Note Length" duration that the output stays 1.
E.g. If "Note Length" is 1/4 and "Pulse Length" is 0.5 the output stays 1 for 1/8th (of a beat).

**Beat Speed**
*(Value between 0 and 1)*
Determines the frequency of the pulse.

**Note Length**
*(read only)*
The frequency set in "Beat Speed" expressed in fractions or multiples of a beat.

**Ease Out**
*(Value between 0 and ~ in seconds)*
Duration the output takes to ease back to 0 after a pulse.


### Color Picker
Lets you pick a color and output it as CHOP Channels.

#### Parameters
**Color**
An RGB Color

**Alpha**
The alpha value of the color

**Channel Name Prefix**
*(String)*
By default the output channels will be named "r", "g", "b", "a" for the color channels. You can specify a string to prefix the default channel names.


### DMX Map
Lets you map values to CHOP Channels via a Table DAT. This is useful to clearly keep track of the DMX Setup at all times. Takes values between 0 and 1 and outputs integer values between 0 and 255 that can be plugged into a DMX Out CHOP.

#### Parameters
**Open Mapping Table**
*(Button)*
Click to open the mapping table in a seperate window.

The first column of the mapping table takes the number of the corresponding DMX channel. Must be a list of consecutive integers. If you have empty channels inbetween mapped channels make sure to fill in the missing numbers. 

The second column takes a python expression pointing to the value the channel will get.

The third column takes a fixture name. Just for clarity. Has no effect. 

The fourth column takes a channel description. Just for clarity. Has no effect. 

## How to contribute
…stub…


