# jumpSynth
trampoline-based synth built with Bela
Watch the video here: https://youtu.be/qDNtRO8HQ2M

Look at the photos for reference on the hardware.

The synth part is a Pure Data patch running on a Bela. It's a kind of silly synth with 8 analog control inputs.
https://puredata.info
https://bela.io

The synth plays a sequence of notes from an array in a loop. With each "button" press from the trampoline it plays the next note.

There is a button for randomizing the notes.

The knob controls on the synth are as follows:
1. Volume
2. Note release length (decay)
3. Delay feedback amount
4. FM mod amount
5. FM mod index
6. "crunch"
7. Pitch offset
8. Pitch range

I found that these eight controls provided a nice balance of fun and control. You may disagree.

The 8 knobs are connected directly to the Bela analog inputs. The Bela is powered by a USB battery pack.

The audio output runs into a stereo amplifier built out of two 386 chips. This is based on the "Ruby" circuit, but without a volume control or input buffer: https://www.electrosmash.com/ruby-amp-analysis

The amp is powered by a separate USB battery pack, because if both the Bela and amp were plugged into the same pack there was crazy noises.

The trampoline sensor is made out of copper tape. You can watch a video on how to make it here: https://youtu.be/28DZphxIRe8

The main difference between that video and this code is that in this instance the trampoline is connected directly to the Bela.

This was made as part of my position as Game Designer in Residence at MICA. 
gamelab.mica.edu
yannseznec.com

Get in touch if you have any questions: yann@yannseznec.com or @yannseznec on twitter.
