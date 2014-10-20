Recipes and Ideas
=================

Autopanner
----------

- Take the main outputs from G8. If possible, mix the stereo outputs down to mono (Your DAW probably has a utility for doing this.)
- Pan that track towards one channel.
- Take the reject outputs, mix them down, and pan them towards the opposite channel.
- **For Transient-based Autopanning**, use the "Regular Gating" mode and set the Threshold to a useful value. Your Attack, Release, and Hold times will control how quickly the pan occurs after the threshold is crossed.
- **For Regular Autopanning**, use the "Cycle" mode and set the Threshold to its minimum value. Again, the Attack, Release, and Hold times will control the panning envelope.
- For either above mode, the Attack and Release times give you separate control over how quickly the audio pans to one channel and how quickly it pans back. It is a rather dynamic effect!


Tremolo
-------

- Set G8's behavior to "Cycle" (instead of "One-Shot" or "Regular Gating").
- Set the Threshold to its minimum value. You should hear a dramatic tremolo effect.
- For a softer tremolo effect, adjust the "Reduction" value.
- Attack, Release, and Hold settings will affect the tremolo's speed.


Granulation/AM Synthesis
------------------------

- Set up the Tremolo patch described above.
- Set the Attack, Release, and Hold settings to extremely low values. When you can no longer hear the individual cycles, you have achieved AM Synthesis.
- To space the grains out more, increase the "Delay" setting.


Bouncing Ball MIDI Generation
-----------------------------

- G8 does not need to receive audio for this effect to work.
- Set the threshold to its minimum setting.
- Change G8's behavior mode to "Cycle". The gate meter should be jumping up and down.
- Connect G8's MIDI output to an instrument that you would like to trigger (For more detailed instructions, please see the section on "Using G8 In Your Host").
- You should now hear the instrument triggering at a regular rate. For a more rapid bounce, decrease the Attack, Hold, and Release times.
- Once you have a bounce setting that you like, increase/decrease the Delay parameter.


Percussion Synthesizer
----------------------

- Set G8's behavior to "One-Shot".
- Run a synthesizer into G8. A great starting patch is a simple mix of a sine tone and white noise.
- Set G8's Attack time to about 10 ms. Set the Hold to 0 ms and the Release to around 100.
- Set G8's Threshold to an appropriate setting.
- Each time you play a note on the synth, G8 will apply its envelope. Since G8 is capable of creating extremely short envelope segments, it makes a great alternative to some synths' less flexible built-in envelope generators.
- For more fun, set G8's behavior to "Cycle" for repeated percussion.

