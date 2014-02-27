dualarduinoboy
==============

This is the hacked version of the arduinoboy, to be able to control 2 DMGS with a single arduino boy (without using dmg07).  Further hacking will be implemented (probably... if I get creative :S)

Three hacks are planned.

1. PENDING. Dual SlaveMode, which is to hack the Slave mode to be able to control 2 DMGS as Slave from and external midi clock.

2. PENDING. Dual MidiOut, which is to hack the MidiOut mode to SEND midi notes to an external midi devide..., right now its almost discarded this option since I would need to first sync both DMGs in someway in Midiout mode (currently unsupported in all lsdj versions...)

3. TESTING. Dual mGB, this is to be able to use 2 DMGs on 8 different midi channels for an 8 voice gameboy synth experience (thru midi...)

Right now the channels are hardcoded to 1-10.

Right now all the midi message from channesl 1-10 are broadcasted to BOTH gameboys, so the midi channels on each mGB needs to be configured properlly, i.e. DMG1 use mGB with midi channels 1-4 and DMG2 use mGB with midi channels 6-9.

While I understsand this is a crappy way to do it, its also interesting if for example you want to have a SUBOSCILLATOR on each DMG voice... you can achieve this by detuning the mGB of one DMG, so for example if the PULSE1 voices of BOTH mGBs are configure on the same channel you can detune (or change any other param on the same channel) and have some sort of polyphony.

===============

For the original Arduinoboy from Trash80 please go to

https://code.google.com/p/arduinoboy