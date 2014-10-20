Additional Features and Modes
=============================

Alternate Gate Behaviors
--------------
Cycle Mode and One-Shot Mode, are variations on G8's default gating behavior, each of which change the way in which the gating envelope will be applied while the gate is "open" (i.e. the input signal is above the threshold level). 

**Cycle Mode**: 

In Cycle Mode the gating envelope will continuously cycle through each of its stages- Attack, Hold, Release, and Delay (optional). Each of the gating parameters control the length of its corresponding portion of this envelope, and the cycle will be repeated until the input signal falls below the threshold level triggering a final release. The speed of each cycle is the sum of the lengths of all four segments (Attack, Hold, Release, and Delay). 

Cycle Mode is useful for creating effects such as amplitude-sensitive tremolo (i.e. when the guitar gets loud, add tremolo), especially in combination with variable reduction amounts. If the envelope lengths are set very low (< 50ms), you can create AM synthesis where the length of the entire cycle functions as the carrier frequency. Similarly, if the delay time is increased while the rest of the envelope values remain very low, you can create granular synthesis where each cycle is heard as an individual sound grain. 

**One-Shot Mode**:

One-Shot Mode is a variation on Cycle Mode, where the gating envelope only fires a single time whenever the input signal goes over the threshold level. The envelope runs through the Attack, Hold, and Release stages immediately, no matter how long the incoming audio is above the threshold for. The envelope will not fire again until the audio has dropped below the threshold and risen above it again. One-Shot mode works best on non-layered sounds, such as an individual drum channel. You can use One-Shot mode, for instance, to drastically alter the character of a snare hit, or to turn a more sustained synth part into percussion tones.

**Additional Notes**:

When in Cycle or One-Shot Mode, G8 will generate a MIDI out note whenever the envelope is triggered. Using this feature in One-Shot Mode is a great way to replace drum hits with another source. In cycle mode, you can use it to create MIDI rolls, automatic bouncing balls, and other otherwise difficult to program flourishes. 


Reject Outputs
--------------

One of G8’s most innovative features is its ability to create “Reject Outputs” when used in four-channel mode. The Reject Outputs are a set of auxiliary outputs that output the sound that is currently being blocked by the gate. If this is hard to conceptualize, mixing together the gated signal and the Reject Outputs will give you back your original signal.

This opens up all sorts of creative mixing possibilities using a technique that we call “amplitude splitting”. This allows you to create non-linear (amplitude dependent) effect chains using any other plug-in you wish.
For a simple example, you could create an amplitude dependent auto-panner. Simply mix the main outs down to one channel, and the Reject Outputs down to another. If you are creating a four-channel mix, this is an easy and flexible surround auto-panner!

For more information on how to connect the Reject Outputs in your DAW, please refer to the section “Using G8’s Sidechain Inputs and Reject Outputs”. If your host doesn’t support G8’s four-channel layout, then please refer to the next section on using the “Flip Mode”.


Flip Mode
---------

When “Flip Mode” is active, the main outputs and the Reject Outputs are swapped. This is useful for a number of reasons. First, if your host does not support G8’s four-channel mode, then this will still give you access to G8’s Reject Outputs. Second, this mode is visible to automation! This allows you to increase the complexity of your Reject Output effect chains by switching between the two modes. Third, it allows you to simply use the Reject Outputs if you have no use for the main outputs.

Why would you want access to only the Reject Outputs? Well, one of our favorite uses of the Flip Mode is to use G8 as a bizarre compressor! To achieve this, activate Flip Mode, and then change the amount of reduction that G8 is using. There are many other wild effects waiting to be discovered in this mode, especially in combination with G8’s alternate behaviors.


Expert Mode
-----------

Expert Mode is an optional mode that provides more in-depth control for advanced analysis situations. In this mode, you have access to the gain of each individual channel, along with the ability to filter the analysis signal. You also have the ability to change between different modes of analysis.

To get you started, here are some ideas for how to use Expert Mode:

- Use the filters to remove noise from your analysis signal. You can remove clicks and pops from your analysis signal to make sure that they don’t open the gate at the wrong moments.
- Control an uneven stereo signal by applying separate gain to each channel or setting Analysis Mode to “Average”.
- Create a mix of your main input and external sidechain input. Balance these correctly to create unusual gating polyrhythms.
- For even more unusual gating behavior, change the analysis mode to “Average” and use two very different input sources.


MIDI
----

