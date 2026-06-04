
# Signal Chain

stuff about how the audio signal is routed/processed



---

# FX

## Equalization (EQ)

EQ is one of the most common and useful effects you will use/encounter when mixing audio. It is important to understand it well. EQ is a powerful tool that allows you to adjust how loud certain frequencies are. With it, you can attenuate the harsh sounds of speech or instruments, eliminate feedback, boost certain regions to enhance clarity, etc. 

There are many kinds of equalizers. Most commonly, you will work with a `Parametric Equalizer` (PEQ). This style of EQ has a graph view showing the frequencies on the x axis and level on the y axis. Most PEQs typically have 4 bands which control the level of the frequencies they are set to. Each band has 3 parameters: `frequency`, `gain`, and `Q`. Of these parameters, `frequency` and `gain` are probably the easiest to understand. They represent which parts of the sound the band affects, and whether it makes that range quieter or louder. Each band affects a range of frequencies, and the width of the range is determined by the `Q`. With the `Q`, one can adjust whether a band is narrow (say, to notch out feedback), or broad (maybe to boost a range of higher frequencies in a voice for a brighter sound).


`insert photo`


The other form of EQ is called a `Graphical Equalizer` (GEQ). In principle, the GEQ does the same thing as the PEQ, but instead of bands, the signal is split into discreet ranges ~10-50Hz wide. The user can use a fader to adjust how loud that range of sound is. This is useful for pinpoint adjustments and taking away feedback on a podium microphone for example, leaving the PEQ for broader adjustments to the tone of the sound. 



### Low-Cut/High-Pass Filter (HPF)

The HPF (as it is often labelled) is a form of EQ which rolls off low frequencies, completely removing the very lowest components of a sound. You can usually adjust how steep the cutoff point is from a gradual transition to a sharp fall as well as where the roll off begins. 

HPFs are useful for removing rumbly sounds (typically <80Hz) which do not contribute to the tonal character of things like speech or an instrument, being more like distracting noise which muddies the mix. It is usually a good idea to apply a HPF to most signals (especially speech). The exception to this is if the instrument/thing being processed is explicitly providing an intentional low signal (i.e. a bass guitar, kick drum, etc.) in which case you probably shouldn't add a low-cut.

`insert photo`



>[!example]
>An acoustic guitar, for example, is usually not playing in very low registers as that is the bass' territory. Most of the strings on a guitar are tuned around 100-400 Hz, with most of the "voice"/character of the guitar around 600-2000 Hz. Higher frequencies responsible for overtones and brightness and such. However, a rumbly signal will almost always be present. It is a safe bet to cut out the lowest frequencies as the guitar is likely strumming in higher registers. Doing this allows the bass instruments to play with less interference; it gives them "more room in the mix."
>
> `insert photo`

<br>

</br>

# Limiter

A limiter is a tool which allows you to set the maximum volume of a signal. It ensures that no sound exceeds the set threshold. If a signal exceeds the volume threshold, it is trimmed/capped at that volume. This is useful to ensure there will not be any deafening sounds in case somebody drops a microphone or a musician unplugs their instrument causing a loud pop or something.


<br>
</br>
## Compression

Compression is another extremely important audio effect you will see everywhere. It is similar to the [[Audio Processing#Limiter|Limiter]] in that it is also used for controlling dynamics, however it is slightly different. Instead of chopping a signal's volume to the threshold, a compressor *attenuates* any signal which goes above the threshold. Once a signal passes the threshold, the compressor turns on and makes the signal quieter by a certain `ratio`. 
