MUS172 HW3: Polyphony - Logan Kirkendall

This folder contains the necessary patches for polyphonic synthesis via MIDI.

Usage:
Open main.pd to view the main patch. This patch is intended to be used with a MIDI device. For a virtual midi, I use VMPK with loopMIDI.
There are 8 individual voice controls that are available. At the top of each voice channel is a voice selector. I'd recommend leaving this alone unless you'd like to change exactly which voice is occupied with your waveform settings. Overlapping voices will only use the settings of the last voice modified. Any voices unselected will have default values, or values that were previously entered into that voice.
Each voice has the ability to have different waveforms, lengths, octave shifts, and full ADSR envelopes. In the bottom left is a control for changing all note lengths together, so that you can have an easier time with polyphony.
The voice number used by the note you play increases every time you play a note, wrapping back to 1 after the 8th voice is played. You can play up to 8 notes simultaneously until a new note overrides the oldest note played.
There is also universal bend support. From whatever midi device you use, the bend control changes the overall pitch of all voices, from -2 octaves to +2 octaves. 
On the left is a VU meter and volume control. By default, the VUM prevents clipping. 
Spectrogram by Thomas Musil (MIT License)