Controls
========

Main Controls
-----------------

.. image:: /images/sandman.png

**Delay Time**:
Sets the length of Sandman's delay buffer. This ranges from 5 milliseconds to 5 seconds. This control is exponential to allow easy manipulation of smaller delay times.

**Sample Rate**:
Controls the sampling rate of Sandman's DSP. Unlike "sample/bit crusher" effects, this control literally affects the speed of Sandman's audio processor. When dropping the sampling rate, you will hear a combination of pitch-warping and lo-fi signal degradation. Without any locks enabled, changing the sampling rate will change the effective size of the delay buffer. As an example, a 400 ms delay will loop every 800 ms when the sampling rate is at 50%. If locks are disabled, the delay time's value label will display the affected value.

**Tempo Sync**:
Enables syncing of Sandman's delay time to your DAW's tempo. For instance, you can create 8th-note echoes perfectly in time with your project's tempo. "T" means "triplet", and "D" means "dotted". Please note that enabling tempo sync does not prevent the sampling rate from affecting the delay time. If you want the delay buffer to always be tempo synced, you must enable both Tempo Sync and Lock Delay Time. Also please note that Sandman's delay buffer size maxes out at 5 seconds at 100% sampling rate. If a specified time unit is longer than 5 seconds, Sandman will default to five seconds. You will only encounter this behavior at extremely slow tempos (Whole notes at 60 BPM would take four seconds, for instance).

**Sleep**:
Freezes the delay buffer. No new information will be written to the delay buffer. This effectively takes the contents of the delay buffer and forces it to loop until "Sleep" is disabled. Once slept, the loop is not affected by the "Filter" or "Feedback" controls, but will be affected by changes to the sampling rate.

**Start/End**:
These controls affect the start and end points of the frozen delay buffer. If locks are disabled, changing these points will affect the playback time of the frozen buffer.

**Lock Delay Time**:
This lock will force the delay buffer to remain the same size, no matter what the sampling rate is. As an example, a 400 ms delay buffer will still take 400 ms to loop, even at a 25% sampling rate. Use this lock if you would like to maintain a specific loop tempo, but want to explore unusual manipulations of the sampling rate.

**Lock Frozen Buffer**:
This lock will force the frozen buffer to maintain its length, no matter where the start and end points are. As an example, a 400 ms delay buffer will always take 400 ms to complete, no matter where the start and end points are. As a side effect, moving the start and end points will affect the pitch of the frozen buffer. Enabling both locks and turning on a lot of modulation can result in some incredible, unusual effects. Try it out!

**Dirt**:
When enabled, this adds an amount of pink noise to the delay buffer depending on the sampling rate. At 100% sampling rate, this will add no noise. At lower sampling rates, this contributes to a lo-fi feeling. With high feedback and Dirt enabled, you can get a larger accumulation of noise in the buffer.

**Feedback**:
Affects the volume of the delay buffer written back into itself. Commonly, you would use this to control the number of echoes that you hear. With short delay times and high feedback, you can create unusual string-like sounds from percussive sources. Feedback doesn't affect anything while the delay buffer is in Sleep mode.

**Filter**:
Applies a low-pass filter to the feedback path. Use this to remove a build-up of hissy high frequencies, or to give the echoes an underwater or "room next door" type of feel.

**Dry/Wet**:
Control the balance between the unaffected "dry" signal and the delayed "wet" signal. Please note that the "gain" knobs do not affect the level of the dry signal.

**In Gain**:
Boosts the level of the audio being written to the delay buffer.

**Out Gain**:
Boosts the level of the output of the delay buffer.


Modulation Controls
-------------

.. image:: /images/sandmanmod.png

To access the modulation menu, click the arrow on the bottom left corner of Sandman.

The modulation menu contains two LFO's with the following waveforms:

- Sine
- Triangle
- Saw Up
- Saw Down
- Sample & Hold

Each LFO is unipolar, meaning that they provide one direction of modulation only. Five sliders on each LFO allow you to set modulation destinations and depths. The center of each slider is the current knob value for each modulation destination. The LFO can add either a positive or negative modulation amount to that value.

**Sync**:
Turns on Tempo Sync for the LFO. When Tempo Sync is on, the rate of the LFO is locked and will not be affected by the Sample Rate. When the LFO is not tempo synced, its speed will be affected by the Sample Rate.
