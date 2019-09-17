# Patch Analysis

One of the most important skills to develop as a synthesist is  self-sufficiency.  No matter how much you think you know, you will never know everything!  Knowing *what to do* when you don't know something is the most valuable tool you can have!  This assignment will help you develop that intuition.

Your task is to break down the patches in the included folders. There are further instructions within the patch, as well as a guide for analyzing the patches included below. You may also refer to Allen Strange's [Rapout Approach to Electronic Instrument Configurations](../rapout.pdf) for more guidance.

Once you think you have a good sense of what is happening in each patch, please look over the annotated version which explains what every part of the patch is doing!

If you encounter a module you do not understand, try right-clicking it and hovering over the `Plugin` submenu to find the `Manual` link.  You can also try searching the internet for more info on that type of module.  There is one module in Patch 2 which will likely be unfamiliar - but do not fret, you can figure it out!  Part of learning about synthesis is learning *how to learn* what you do not know.

Do not forget to make sure you sound card is set correctly and that the volume is turned on!

## Patches

[Patch 1](./patch_1/patch_for_analysis.vcv)

[Patch 1 Annotated](./patch_1/patch_annotated.vcv)

[Patch 2](./patch_2/patch_for_analysis.vcv)

[Patch 2 Annotated](./patch_2/patch_annotated.vcv)

Or, download all the files as a .zip by going to this link and pressing "download":

[Patch Analysis Files (.zip)](./Patch-Analysis.zip)

## Analysis Principles

When looking at a patch - whether in a tutorial video, on a forum, with a collaborator, in this class, or even after you have been patching in a flow/experimental-state for a while - it can be quite overwhelming to figure out what is going on.  However, if you make the task of analyzing a modular synthesis patch more... modular... it becomes much more manageable!  Here are some useful tools to help you break down the task of "analyze this patch" into smaller parts.

### Sound

This is about making sound - so start by focusing on the audio pathways.

1. Figure out where the final output of a patch is, and trace the audio signals backwards from there: which modules are feeding audio signals to the output?  In turn, which modules are feeding *those* modules?  Work your way backwards to figure out where the original sound generators are.
2. Once  you have a sense of the audio pathways, try to figure out what each stage of the audio path is doing: Generating audio?  Processing audio?  Mixing audio?  What purpose does each stage have in shaping the sound?
3. Focus on one stage at a time, and make a list of what are the modulation points for each stage (i.e. what parameters are being modulated), and get a sense of what the types of modulation are for each parameter (e.g. sequences, LFOs, envelopes etc).
4. Are there any feedback pathways?  Are audio signals ever used as modulation sources, e.g. for FM synthesis?

### Control Voltage

But it is also about composing time and space - turn your attention towards the modulation and composition structure of the patch.  

1. Is timing important to the patch?  If so, how is it created?  Is there a single leader clock which many modules are synchronized to?  Are there multiple independent, unrelated clock streams?  Are LFOs being used to create the clock streams, or other types of clock generators?  Are clock streams sent to clock modulators to create new gate patterns?
2. How are gates created (if they are needed in the patch)?  What module generates the gate patterns?  How is that module controlled?  Are these patterns controlling individual notes, or larger transitions across a whole patch?
3. How are pitch CV signals generated (if needed in the patch)?  Sequencers?  Pattern generators?  Sample+Hold?  Are quantizers used?
4. How is modulation used to design sound, space, and time?  Are there envelopes being applied to parameters?  Random step sequences?  LFOs?  Is modulation processed before being applied to the parameters? Does a given modulation signal act on the micro-, meso-, or macro-timescale?  Does a given modulation signal change compositional structure or audio processing?

### Interaction

And finally, composing with a modular is also about interacting with a system.  

1. What points of interaction/improvisation are embedded within the patch?  
2. How can the system be guided in real-time?
3. Can the patch be "live-coded" - i.e. are there patch connections which are made or removed in real-time?
4. Where does the system fall along the axes of "generative/self-playing," "real-time improvisation," and "completely through-composed?"