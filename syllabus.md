# Intro to Modular Synthesis @ Pioneer Works

0. [Pre-Class Prep Work](#Pre-Class-Prep-Work)
1. [Week 1: Modular Thinking](#Week-1)
2. [Week 2: Creating Events](#Week-2)
3. [Week 3: Timbre and Time](#Week-3)

## Pre-Class Prep Work

1. Install [VCV Rack](vcvrack.com) on your laptop computer.  Once installed, log-in by clicking the `Library` dropdown in the toolbar and using the credentials `itmspw@gmail.com` and password `synthesis`.  Once logged in, press `Library > Update all`.
2. Read [Chapter 0 - Introduction to Modular Thinking](./Chapter-00/chapter00.md).  We will be going over all this (and more!) in our first class.  
3. Review these very short web demos on [pitch](https://learningsynths.ableton.com/making-changes/amplitude), [amplitude](https://learningsynths.ableton.com/making-changes/pitch) and [playing with both](https://learningsynths.ableton.com/making-changes/play-with-amplitude-and-pitch).
4. Please download the VCV Rack Lab patches for [Chapter 1](./Chapter-01/patches/ch01_vcv_labs.zip), [Chapter 2](./Chapter-02/patches/ch02_vcv_labs.zip) and [Chapter 3](./Chapter-03/patches/ch03_vcv_labs.zip) - we will be doing these in class, so please have the files downloaded on your computer when you arrive.  Right- or opt-click the links and select `Save as ...` to save the .zip files.
5. Remember to bring your laptop, headphones, and notetaking materials!



## Week 1

### Modular Thinking

*This week, we will learn about the physics of sound and the fundamental concepts of modular synthesis like signal flow, patching, control voltage, and modulation.  We will also get familiar with VCV Rack, an open-source modular Eurorack modular synthesis emulator.*

### Agenda

- **Introductions**
- **Course Overview**
- **Modular Thinking**
  - The Parameters of Sound
  - The Electronic Transmission of Sound
  - So What's a Patch?
  - Control Voltage and Modulation
- **Modular Building Blocks**
  - Oscilloscopes: Visualizing Voltage
  - Oscillators: Frequency and Amplitude
  - Attenuators & Voltage Controlled Amplifiers: Amplitude Control
- **Break** (5 minutes)
- **Lab - Introduction to VCV Rack**
  - Adding modules
  - Deleting modules
  - Using patch cables to connect modules
  - 'Multing' patch cables
  - Using the VCV Rack oscillscope to visualize constant voltages, LFOs, and Oscillators
  - Getting sound out of VCV Rack.
  - Using VCOs, LFOs, Attenuators/Attenuverters, and VCAs

### Key Vocabulary

[Click here for definitions](./glossary.md#week-1)

Pitch, Timbre, Loudness, Voltage, Signal, Input, Output, Control Voltage (CV), Modulation, Audio-rate Voltage, Oscilloscope, Oscillator, Voltage-Controlled Oscillator (VCO), Low-Frequency Oscillator (LFO), Amplitude, Attenuator, Voltage-Controlled Amplifier (VCA), Hertz (Hz), Frequency, Inverter, Attenuverter, Unipolar Voltage, Bipolar Voltage, Signal Flow, Modulation Depth

### Homework

| Type                  | Link                                                         |
| --------------------- | ------------------------------------------------------------ |
| *Review*              | [Vocabulary]()                                               |
|                       | [0: Introduction to Modular Thinking](./Chapter-00/chapter00.md) |
|                       | [1: Introduction to VCV Rack and Generating Voltage](./Chapter-01/chapter01.md) |
|                       | [2: Voltage-Controlled Oscillators, Attenuversion, and Control Voltage](./Chapter-02/chapter02.md) |
|                       | [3: Voltage-Controlled Amplifiers](./Chapter-03/chapter03.md) |
|                       | Powerpoint [[.pptx](./powerpoints/week1_powerpoint.pptx), [.pdf](./powerpoints/week1_powerpoint.pdf)] |
|                       |                                                              |
| *Suggested Listening* | Blawan - *Wet Will Always Dry* (2018) - [[*Direct Download*](https://www.dropbox.com/sh/tfi694y0woky5q6/AACL5mXmbMi_ysIDs3Vl6BiHa?dl=0), [*Spotify*](https://open.spotify.com/album/0tAeHP4BXGplGcD6rdYXjy?si=8quFgbnMQbO3RkgIuDttPQ)] |
|                       | Golden Retriever - *Seer* (2014) - [[*Direct Download*](https://www.dropbox.com/sh/uyns2lekqq0bkqy/AACYN7TySx8I5ULtoiQ3UwRva?dl=0), [*Spotify*](https://open.spotify.com/album/5Jfbs3LoaxLpRPIr8bNRlT?si=zvs52SmcTgqzSI64IYt-gA)] |
|                       | Laurie Spiegel - *The Expanding Universe* (1980) - [[*Direct Download*](https://www.dropbox.com/sh/dj3k06iecvet0x7/AADFZ8ILLy15hx-3d0GwHPAva?dl=0), [*Spotify*](https://open.spotify.com/album/2rD0SKiBImTKNhRtRVLsdU?si=LtdM5kpdS6G_2FB7_W7MaA)] |
|                       | [Suzanne Ciani on Modular Synthesis (YouTube)](https://www.youtube.com/watch?v=QRx-YdqHLus&t=250s) |





## Week 2

### Creating Events

*This week will introduce you to the core tools for creating events and layering modulation and sound in the modular synthesis world: triggers, gates, clocks, envelopes, triggers, and mixers.  We will also explore tonality and basic music theory as they relate to tuning synthesizers: intervals, scales, the V/Oct standard, and quantizers.*

### Agenda

- **Review** 
  - Voltage as Sound
  - Control Voltage
  - Voltage-Controlled Oscillators and LFOs
  - Attenuators and Attenuverters
  - Voltage Controlled Amplifiers
- **Creating an Event**
  - Gates and Triggers
  - Clocks
  - Envelopes
- **Creating a Melody**
  - Scales, Pitch, and Frequency
  - Volt/Octave
  - Sequencers
  - Quantizers
  - Sample & Hold and Slew Limiters (if time permits)
- **Mixers**
  - Control Voltage
  - Audio
- **Break** (5 minutes)
- **Lab - Creating Harmonized Sequences**
  - Using Clocks to drive CV and Gate sequencers
  - Using Quantizers to create V/Oct CV
  - Using Envelope Generators and VCAs to shape events
  - Using Mixers to combine multiple audio sources
  - Using Mixers and VCAs to alter CV sequences
- **Modular Thinking: Understanding a Patch**
  - Top-down analysis
  - Bottom-up analysis
  - Dealing with the unfamiliar/unknown

### Key Vocabulary

[Click here for definitions](./glossary.md#week-2)

Trigger, Gate, Triggers, Rising-Edge, Trigger/Gate Threshold, Gates, Pulse-Width, Clocks, Clock Modulation, Envelope, Envelope Generator (EG), Attack, Decay, Sustain, Release, Interval, Octave, Scale, Volt-Per-Octave (V/oct), Sequence/Sequencers, Quantizer, Unity Mixer, Mixer

### Homework

| Type        | Link                                                         |
| ----------- | ------------------------------------------------------------ |
| *Review*    | [Chapter 04: Gates, Triggers, Clocks, and Envelope Generators](./Chapter-04/chapter04.md) |
|             | [Chapter 05: Sequences, Quantizers, Scales and Volt-per-octave, Quantizers)](./Chapter-05/chapter05.md) |
|             | [Chapter 06: Mixers](./Chapter-06/chapter06.md)              |
|             | [Patch Analysis](./Assignments/Patch-Analysis/patch-analysis.md) |
|             | [Module Breakdown](./Assignments/module-breakdown.md)        |
|             | Powerpoint [[.pptx](./powerpoints/week2_powerpoint.pptx), [.pdf](./powerpoints/week2_powerpoint.pdf)] |
|             |                                                              |
| *Suggested* | [Try out some "Exploration Ideas"](./Assignments/exploration-ideas.md) |
|             | [Come to *Modular on the Spot* @ Nowadays](<https://www.facebook.com/events/nowadays/signal-flux-hosts-modular-on-the-spot/2065950230178187/>) |
|             | Morton Subotnick - Silver Apples of the Moon (1967) - [[Youtube](https://www.youtube.com/watch?v=3G1hRNLlYpg)] |
|             | Wendy Carlos - Switched on Bach (1968) - [[Youtube](https://www.youtube.com/watch?v=fVxGpN8B4BQ)] |
|             | Mort Garson - (Mother Earth's) Plantasia (1976) - [[Youtube](https://www.youtube.com/watch?v=l0vrsO3_HpU)] |
|             | Kaitlyn Aurelia Smith - In the Studio w/ Fact Mag [[Youtube](https://www.youtube.com/watch?v=95UvPlhjbE4)] |

## Week 3

### Sculpting Timbre and Time

*This week we will explore tools for shaping timbre via additive / subtractive synthesis, wavefolding, filters, and time-based effects. We will also learn how to achieve more complex and generative patterns with clock modulation, Euclidean rhythms, polyrhythms, S+H, slew limiters, and controlled randomness.*

### Agenda

- **Review** 
  - Creating an Event
    - Gates, triggers, clocks
    - Envelope generators
  - Creating a Melody
    - Scales, pitch, frequency
    - Volt/octave
    - Sequencers
    - Quantizers
  - Mixers
    - Audio
    - Control voltage
  - Patch Analysis 
  - Module Breakdown
- **Controlling Timbre** 
  - Spectrum & Waveshape
  - Filters
  - Wavefolding
- **Effects** 
  - Delay
  - Reverb
  - Distortion
- **Pattern Generators** 
  - Clock Modulators / Euclidean Rhythms
  - Phasing LFOs and Polyrhythms
  - Controlled Randomness/Chance
- **Break** 
- **Lab** 

### Key Vocabulary

[Click here for definitions](./glosary.md#week-3)

Fourier Analysis/Synthesis, Harmonic, Partial, Spectrum, Frequency Domain, Spectrogram, Time Domain, Waveshape, Noise, Voltage-Controlled Filter (VCF), Subtractive Synthesis, Cutoff Frequency, Resonance, Wavefolding, Delay, Reverb, Distortion, Dry Signal, Wet Signal, Dry/Wet Clock Modulation, Euclidean Rhythms, Reset, Polyrhythms, Phasing, Sample and Hold, Slew Limiters

### Homework

| Type        | Link                                                         |
| ----------- | ------------------------------------------------------------ |
| *Review*    | [Chapter 07: Spectrum, Waveshape, Filters, Wavefolding, Noise](./Chapter-07/chapter07.md) |
|             | [Chapter 08: Delay, Reverb, Distortion](./Chapter-08/chapter08.md) |
|             | [Chapter 09: Sample+Hold and Slew Limiters](./Chapter-09/chapter09.md) |
|             | [Chapter 10: Clock Modulators and Rhythm](./Chapter-10/chapter10.md) |
|             | [Visit Control](./Assignments/Visit-Control/visit-control.md) |


| *Suggested* | Surgeon – From Farthest Known Objects (2016) [[*Spotify*](https://open.spotify.com/album/3y3v158VcH2ENOIdKGImca?si=GCrFwvIAT1axTA49gEGERA)] |
|             | Venetian Snares – Traditional Synthesizer Music (2016) [[Bandcamp](https://venetiansnares.bandcamp.com/album/traditional-synthesizer-music), [*Spotify*](https://open.spotify.com/album/7nqOcV9Ilnrnuzwvq77xn4?si=sraSdOMRQmyWs6w70Q1h1g)] |
|             | Emily Sprague – Water Memory (2017) [[Bandcamp](https://mlesprg.bandcamp.com/album/water-memory), [*Spotify*](https://open.spotify.com/album/7GFnprDHbH3BkxjCiOH0k6?si=OpynT78DTKatBdXWT6rdxg)] |
|             | Robert Aiki Aubrey Lowe – Exploratorium Performance [[YouTube](https://www.youtube.com/watch?v=Jr_8RmjXK54)] |
|             | Caterina Barbieri – Boiler Room [[YouTube]](https://www.youtube.com/watch?v=W25FTlO42VY) |
|             |                                                              |
