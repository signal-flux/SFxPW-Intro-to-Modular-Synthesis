[Week 1]: #Week-1
[Week 2]: #Week-2
[Week 3]: #Week-3
[Week 4]: #Week-4
[Alphabetical]: #Alphabetical



# Key Vocabulary/Glossary

- [Week 1]
- [Week 2]

- [Week 3]

- [Week 4]

- [Alphabetical]

## Week 1

| Term                                  | Definition                                                   |
| ------------------------------------- | ------------------------------------------------------------ |
| *Pitch*                               | How 'high' or 'low' a sound is; each key on a piano corresponds to a different pitch; the primary difference between two notes played by the same instrument (e.g. two different keys on the piano, two different strings on a guitar) is their pitch.  Sequences of pitches can create melodies. |
| *Timbre*                              | The quality or character of a sound; how harsh or clean it is; bright or soft; the primary difference between two notes with the same pitch but played by different instruments is their timbre (e.g. middle C played by a piano, a guitar, or a human voice are all the same pitch, but have different timbres). |
| *Loudness*                            | The apparent intensity of a sound; how loud or quiet it is.  |
| *Voltage*                             | How electricity is measured.  Voltage has a magnitude (e.g. size) and polarity (e.g. positive or negative).  Sound waves can be transmitted as electrical voltages which mirror the sound waves.  Modular synthesizers send audio between modules as voltages; modular synthesizers also use constant or slowly changing voltages to control other parameters of other modules. |
| *Signal*                              | Electrical information transmitted from one module to another over a patch cable; may be audio or control information. |
| *Input*                               | Incoming information/signals are received by a module at its input.  The module determines its output based on the state of its inputs.  Some inputs are *jacks* which you can plug a cable into to feed the input with a signal from another module. Other inputs may be interactive, like knobs, faders, switches, buttons, or touchplates. |
| *Output*                              | Signals leave a module at its output jacks.  Output signals may be sent to other modules, or possibly to speakers to be turned into sound.  The output signals are created based off of each module's individual rules for processing and converting its inputs into outputs. |
| *Signal Flow*                         | The path signals take as they are travel through the system from origin to final destination.  The patch cables carry signals as voltage from outputs towards inputs. |
| *Control Voltage (CV)*                | Control voltage signals are relatively slowly changing and can be used to change a parameter of another module by sending it to the corresponding input.  For instance, control voltage may set the pitch of a sound generating module, or slowly increase and decrease the volume of a sound processing module. |
| *Modulation*                          | Using control voltage to change a parameter on a module (for instance, pitch or loudness) over time. |
| *Audio-rate Voltage*                  | Voltage that changes very quickly (greater than 20 times per second, or > 20 Hertz).  When connected to a speaker, the voltage pushes the speaker cone back and forth very quickly, creating sound waves which we ultimately hear as sound.  Sound generating modules create audio-rate voltages, while sound processing modules expect audio-rate voltage inputs. |
| *Oscilloscope*                        | Used to visualize voltages.  Displays *Time* on the X-axis and *Voltage Amplitude* on the Y-axis.  *Time Scale* is used to zoom in and out along the X-axis, displaying a long swath of time to visualize voltages that change slowly (control voltage), or a narrow band of time to view voltages which change quickly (audio-rate voltage) |
| *Oscillator*                          | Creates a voltage which moves up and down in a repeating pattern.  One repetition of the pattern is known as a *cycle* or a single *oscillation*.  The shape of each cycle is known as the *waveshape*. The time it takes to complete one cycle is known as the *period*.  The number of cycles completed in one second is known as the *frequency*, and is measured in *Hertz (Hz)*, aka *cycles per second (cps)*.  A greater period means a smaller frequency, since each cycle takes longer and thus fewer cycles are completed in one second.  Similarly, a shorter period means a higher frequency.  If the frequency is greater 20 Hertz, the oscillating voltage can be sent to a speaker and turned into sound; as the voltage goes up and down, it pushes the speaker cone back and forth, which in turn pushes air back and forth, creating sound waves.  Higher frequencies corresponding to higher pitches.  Different waveshapes create different timbres. |
| *Voltage-Controlled Oscillator (VCO)* | An oscillator whose frequency can be controlled by an external control voltage.  Usually has a knob which sets the base frequency.  Sending in positive voltages to the *frequency modulation (FM)* input will increase the frequency of the oscillator.  Negative voltages will decrease the frequency.  Some VCOs may also have voltage-controllable waveshape, allowing you to use CV to affect the timbre.  When the frequency is greater than approx. 20 Hz, the oscillation is fast enough to be sent to a speaker and heard as sound. |
| *Low-Frequency Oscillator (LFO)*      | Creates an oscillation which is too slow to be used as sound, but can be used instead to control parameters of another module (for instance, making a sound brighter or darker in a repeating pattern). |
| *Amplitude*                           | How large or small a changing voltage is.  For quickly-changing audio-rate signals, the "amplitude" refers to the maximum and minimum voltage which the signal reaches.  The amplitude of an audio-rate signal determines its loudness.  Two audio-rate signals with identical waveforms but different amplitudes will have the same timbre but different loudness because they push the speaker cones back and forth in the same pattern but to different maximum and minimum displacements.  The amplitude of control voltages is often referred to as the "depth" of modulation. |
| *Attenuator*                          | Changes the amplitude of an incoming signal without changing the shape of it in time; vertically stretches or shrinks a voltage.  A knob sets how much the incoming signal is attenuated (made smaller) before passing through to the output.  Fully CCW corresponds to full attenuation (input signal is not passed, 0V output), while fully CW corresponds to no attenuation (original signal passes through unaffected at its full amplitude).  Since amplitude corresponds to loudness of an audio signal, attenuators can be used to make audio signals louder and quieter.  Can also be used to change the amplitude of control voltages in order to change how much they affect a destination parameter; this is known as controlling the  "depth" of modulation.  When fully attenuated, the incoming control voltage will not pass through the attenuator and will have no affect on the destination parameter (no depth).  When the attenuator is fully 'open', the control voltage passes straight through the attenuator and will fully modulate the destination parameter (maximum depth). |
| *Voltage-Controlled Amplifier (VCA)*  | Like an attenuator, but instead of using a knob to set attenuation, a VCA can use a control voltage to set the attenuation/amplification of an incoming signal to process.Expects two inputs: a voltage to process, and a control voltage which determines how to change the amplitude of the signal to process. |
| *Hertz (Hz)*                          | 1 Hz = 1 cycle completed per second                          |
| *Frequency*                           | How many cycles an oscillator completes in a single second. Measured in Hertz (Hz), aka cycles per second (cps) |
| *Inverter*                            | Flips the polarity of an incoming voltage, but leaves magnitude unaffected: turns positive voltages negative and turns negative voltages positive.  +3.4V becomes -3.4V, and -2.5V becomes +2.5VV. |
| *Attenuverter*                        | Similar to an attenuator, but it can also invert voltages.  At noon, incoming voltage is fully attenuated.  Between noon and CW, attenuation is decreased just like on an attenuator (with no attenuation reached fully CW).  Between noon and CCW, the incoming voltage is inverted before it is attenuated; attenuation of the inverted voltage decreases as the knob moves from noon to fully CCW.  Original signal is passed to the output at its fully amplitude but inverted when the knob reaches CCW. |
| *Unipolar Voltage*                    | A signal which is only positive or only negative, e.g. an LFO whose range is 0V to +8V; alternatively, 0V to -8V would also be unipolar.  *Uni*- means 'one' and *-polar* refers to polarity (positive or negative). |
| *Bipolar Voltage*                     | A signal which can be both positive and negative, e.g. an LFO whose range is -5V to +5V.  *Bi*- means 'two' and *-polar* refers to polarity (positive or negative). |
| *Modulation Depth*                    | The extent of a change in a parameter caused by modulation; how far a parameter under voltage control moves from its normal position. The farther the control voltage pushes the parameter, the greater the  modulation depth. |

## Week 3



## Week 4



## Alphabetical

