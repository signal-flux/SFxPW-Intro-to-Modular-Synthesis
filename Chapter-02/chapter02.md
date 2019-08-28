# 2: Voltage-Controlled Oscillators and Attenuation

This chapter will introduce you to several core building blocks of modular synthesis: the *voltage-controlled oscillator*, or *VCO* for short; the *low-frequency oscillator*, a close sibling of the VCO; and the *attenuator*, *inverter*, and *attenuverter*.

To start, we won't focus too much on the *musical* utility of the various ingredients for modular synthesis.  Instead, we will focus on understanding how they work abstractly so you can build intuition for what they are actually doing, and gain a basic understand of how voltage is turned into sound.  You have to walk before you can run!

When you are ready, move on to the [next chapter](../Chapter-03/chapter03.md)!

## Labs

Right-click (or alt/opt-click) on the links below; then click `Save as ..` to download the two VCV Rack labs.  Make sure you are logged in to the class VCV Rack account before you begin: use credentials `itmspw@gmail.com` (password: `synthesis`) and hit `Library > Update plugins` before you begin.  Once you are logged in and have downloaded the labs/updated your plugins, double-click the first lab in your file browser, or open it using VCV Rack's `File > Open` dialog.  

[Lab 2.1: Oscillation, Frequency, Period, and Waveshape](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_1_annotated.vcv)

[Lab 2.2: Attenuators and Amplitude](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_2_annotated.vcv)

[Lab 2.3: Inverters](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_3_annotated.vcv)

[Lab 2.4: Attenuverters](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_4_annotated.vcv)

[Lab 2.5: Normalling](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_5_annotated.vcv)

[Lab 2.6: Unipolar vs. Bipolar Oscillation](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_6_annotated.vcv)

[Lab 2.7: Getting Sound from VCV Rack - Oscillators, Pitch, and Frequency](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_7_annotated.vcv)- ***do not skip this one!***

[Lab 2.8: Oscillator Waveshape and Timbre](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_8_annotated.vcv)

[Lab 2.9: LFOs, VCOs, Frequency Modulation, and Control Voltage](https://raw.githubusercontent.com/signal-flux/SFxPW-Intro-to-Modular-Synthesis/master/Chapter-02/patches/lab_2_9_annotated.vcv)

You can also go to the page below and click download to get a .zip file containing all the labs for Chapter 2:

[Chapter 2 Labs (zip)](./patches/ch02_vcv_labs.zip)



## Additional Notes

If there is anything you are having trouble understanding in the labs, see if the notes below help! If you want more guidance, comment in the slack, or shoot Izzy or Sam a message!

### LFOs

A *low-frequency oscillator*, or LFO, generates a voltage that changes over time in a periodic (aka repetitive) fashion.  The pattern of how the voltage changes over time stays the same, and is called the *shape* of the oscillator.  The repetition of this pattern is known as an *oscillation*.  An oscillator just generates oscillations!   The height, or maximum level of these oscillations, is known as the *amplitude*.  The duration of time it takes to complete one cycle of this pattern is called its *period*.  The number of cycles it completes per second is called its *frequency*, and is measured in *Hz* (1Hz = 1 cycle completed per second).  An LFO then is just an oscillator that produces a voltage which changes in a pattern at a very slow rate - this makes it ideal as a *control voltage*, or *CV* source for controlling parameters of other modules! 

### Unipolar vs Bipolar

*Unipolar* waveforms are always greater than or equal to `0V`, or always less than or equal to `0V`, but they can never be both positive and negative.  They have one direction (or pole) which they can move towards from 0V, either positive or negative, but not both.

*Bipolar* waveforms can vary around either side of `0V`, meaning they can go back and forth between being positive and negative.  

### Attenuators

An attenuator *attenuates* incoming signals (also called "*scaling*"), meaning it changes their amplitude, but not their overall shape.  The output of an attenuator is always equal to the input  voltage times a scaling factor determined by the attenuator knob position.

`output = input x knob`

Usually, when the attenuator is fully clockwise, the scaling factor 1, meaning the output is just equal to the input.  When the knob is in its middle position (noon), the output is equal to exactly half of the input voltage. When the knob is at its minimum position CCW, the scaling factor is 0, so the output is also 0V.  

Attenuators can be used to make audio signals quieter, since amplitude corresponds to loudness; this is because the amplitude of an audio waveform controls how far a speaker cone moves back and forth, and thus how far our ear drums are pushed by the sound wave which eventually reaches them.

Attenuators can also be used to process control voltage signals; they allow you to control how much a destination parameter is modulated by the control voltage source.  Often, modules will have built in attenuators (or attenuverters) since they are so useful when it comes to precisely dialing in modulation ranges!

### Inverters

Inverters flip the polarity of the input signal. The output of an inverter is always given by this equation:

`output = -1 x input`

### Attenuverters

Attenuverters allow you to change both the amplitude and polarity of an input signal.  They function equivalently to attenuators, but the minimum (fully CCW) position corresponds to a scaling factor of -1, while the maximum (fully CW) position corresponds to a scaling factor of 1.  At noon, the output of an attenuverter will be 0V, since the scaling factor is 0. 

### Normalling

For some modules, it is as if there is a "default" voltage sent into some of a jack even when nothing is plugged in.  As soon as you plug something into the jack, the default voltage gets ignored and the input voltage that was just connected takes over.  However until then, when nothing is plugged in, this default voltage is treated as the input.  

This is known as *normalling*.  This default voltage is said to be *normalled* into the input jack.  Plugging a cable into the jack *breaks the normalled connection* - sometimes we will simplify this by just saying that it *breaks the normal*.  When the normal is broken by a cable, the default normalled voltage just gets replaced with whatever is being sent into the jack via the new cable.

### Oscillators and Sound

Oscillators are simply modules which produce signals that go up and down in a repetitive pattern over time, as discussed in the previous introduction to LFOs.  Before though, we did not actually do anything with this voltage that went up and down.  Here though, we patched it to a speaker, and eventually heard sound once the frequency got high enough.  As the frequency of the oscillation increased, the pitch of the oscillator went up, and the waveform seemed to compress on the scope, as more and more cycles completed for each frame that the scope drew. As the frequency of the oscillation decreased, the waveform seemed to stretch out, and the pitch decreased.  The attenuverter seemed to control the volume of the signal.

All tonal material - i.e. sound material that seems to have a pitch, is characterized by a repeating waveform which pushes air back and forth.  This is precisely what vibrating vocal chords do.  Similarly, the vibrating string of an acoustic guitar transfers its vibrations to the body of the guitar via the bridge, which then amplifies those vibrations in its cavity, and emits the vibrating sound waves out of the sound hole.

When we patch a repeating waveform voltage to a speaker, the voltage pushes a magnet back and forth precisely in sync with the repeating waveform pattern.  The magnet then pushes a speaker cone back and forth, which in turn pushes air back and forth.  The higher the voltage sent to the speaker, the further the magnet pushes the speaker cone from its resting position at `0V`.  The more negative the voltage, the further the magnet pulls the speaker cone in from its resting position.  The oscillating voltage waveform is *transduced* into an oscillating kinetic waveform - i.e. the motion of the speaker cone moving back and forth.  This kinetic waveform in turn is transduced into an acoustic waveform as the speaker cone pushes air - i.e. a waveform that travels through the air as compressions and rarefactions of air molecules.  This acoustic waveform eventually hits your ear drum

Your ear drum then gets pushed back and forth in sync with the original electrical waveform, and your inner ear transduces this motion back into an electrical signal which travels along nerves to your brain, which then, quite magically, you phenomenalize as the experience of sound.

In order for sound to be audible, the air must be vibrating very fast.  For instance, if I high-five the air in front of you, you won't hear the sound of my hand pushing air towards you.  If I push my hand forwards and backwards as fast as I can, you still won't hear it.  If I clap once, you will hear a percussive burst which corresponds to a single wave of compressed air molecules traveling towards you, however you won't hear any pitched sound - this is because the intensity of the wave is strong enough to push your ear drums in very fast and generate a sharp electrical transient in your inner ear, but because it is not a repeating compression and rarefaction of air, you don't hear a pitch.  The harder I clap, the greater the intensity of the sound wave, and thus the louder the sound.  Explosions then are just like really loud claps!

Think back to the experiment at the start of this section - at low frequencies, you just heard a click from the speaker cone moving position very sharply and pushing a column of air abruptly, similar to a clap.  However, once the frequency of the LFO became fast enough, these repetitive compressions of air became frequent enough to merge the clicks into a pitched tone.  As the frequency went higher and higher, the pitch went higher and higher.  Remember, *frequency* just means the number of times an oscillation repeats one cycle of its waveform per second, and it is measured in *Hertz* (1Hz = 1 repetion per second). 

For humans, the point at which oscillations become audible as pitched sound is about 20Hz, or 20 cycles-per-second (i.e. if a click happens 20 times per second, you will hear it as a tone, rather than as a sequence of transients).  Oscillations below that rate cannot be heard as pitches, but they are certainly useful for controlling parameters of other modules, like volume, or even frequency of another oscillator!  Voltages which change slower than 20Hz are typically said to be *control voltages*, or *CV*, which change at *control rate*, due to their usefulness in controlling other parameters on your synthesizer!  Voltages which oscillate faster than 20Hz are typically said to be at *audio rate*.  The edge of human hearing is somewhere between 15kHz and 20kHz (*NB: 1kHz = 1000Hz*), depending on age and other hearing loss factors.  

What determines the loudness of a sound?  Well, we said before that the difference between a clap and explosion was just the intensity with which a single pulse of air is generated.  For oscillations, the height of the waveform determines how far forward and backward the speaker cone moves, which in turn determines the intensity with which air is pushed forwards and backwards.  The greater the height of an audiorate waveform, the louder it will be as a sound!  The height of a waveform is known as its *amplitude*, and is typically measured in *Vpp*, or "peak-to-peak voltage".  This just means the distance from the most positive voltage that the waveform reaches to the most negative voltage the waveform reaches.  Now that you understand amplitude, think about why the attenuverter controlled the volume of the sound you heard!  When you patch an oscillator through an attenuverter, the knob just controls the amplitude of the waveform without affecting its frequency or shape, and so it simply controls the volume!

