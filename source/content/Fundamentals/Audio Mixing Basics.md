
# Signal Chain

stuff about how the audio signal is routed/processed



---

# Signal Processing

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
## Limiter

A limiter is a tool which allows you to set the maximum volume of a signal. It ensures that no sound exceeds the set threshold. If a signal exceeds the volume threshold, it is trimmed/capped at that volume. This is useful to ensure there will not be any deafening sounds in case somebody drops a microphone or a musician unplugs their instrument causing a loud pop or something.


<br>
</br>
## Compression

Compression is another extremely important audio effect you will see everywhere. It is similar to the [[Audio Mixing Basics#Limiter|Limiter]] in that it is also used for controlling dynamics, however it is slightly different. Compressors effectively make the loud parts of a signal quieter, allowing you to increase the volume without blowing out the audience's ears. They are extremely useful when the signal has a high Dynamic Range like in speech or wind instruments. 

>[!example]
>A speaker may talk quietly at times and loudly at others. Without a compressor you must make a decision about what level to set them at: A loud volume will allow audience members to hear their quieter speech, but if they move closer to the microphone or talk louder, it may come uncomfortably loud through the speakers. However, if you set the level down so that the loud parts of their speech are not painful, it may be too hard to hear their voice. It is hard to predict changes in volume, so it is unfeasable to manually adjust levels during the event. 
>A compressor fixes this issue by automatically making the loud parts not so loud, allowing you to increase their volume such that both quiet and loud speech come through at a legible and comfortable volume.

Instead of chopping a signal's volume to the threshold as a [[Audio Mixing Basics#Limiter|Limiter]] does, a compressor *attenuates* any signal which goes above the threshold. Once a signal passes the threshold, the compressor turns on and makes the signal quieter by a certain `ratio`.  For example, if a signal exceeded the threshold by 10dB at a ratio of 2:1, it is compressed such that it now only exceeds the threshold by 5dB. Similarly, a ratio of 5:1 means the signal now exceeds the threshold by 2dB. A ratio of 1:1 does nothing to the sound and is equivalent to no compression. Remember that the compressor will not activate until the threshold is exceeded. 

### Compressor Parameters

Most compressors will have the following settings/parameters: Attack, Release, Threshold, Ratio, Knee, and Gain/Makeup. Threshold and ratio were already discussed and fairly straightforward. 

Attack is also fairly easy to understand: it represents how quickly it takes for the full attenuation to take effect. It is usually a few μs (microseconds) to tens of ms. Release similarly dictates how long it takes for the compressor to relax/"let go" to the original volume once the signal goes below the threshold again. The release typically ranges from tens to hundreds of ms. A quick attack is useful when sharp transients are present such as in drums, but it may sound a bit harsh or unnatural on things like speech to have a fast attack and release. You will hear the compressor going on and off repeatedly which may sound odd or artificial. Conversely, too long of either attack or release could lead to a weird pumping sound and leave the signal sounding a bit squashed. 

The Knee dictates whether a compressor will turn on *only* when the threshold is crossed, or smoothly transition to being on as the volume approaches and exceeds the threshold. The knee is typically either hard or soft. A soft knee is typically used on things like podium mics to give a more natural feel to the effect. A hard knee may lead to detectable moments when the compressor turns on and sounds a bit awkward.

Gain/Makeup is simply a flat increase to the signal to "makeup" for the reductions in volume. 

`insert photos`


## Pan

Panning/Balance is whether the audio is weighted more towards the left speakers, right speakers, or split equally between them (center). All panning does is change the amount a sound comes through each side. This can be useful if your venue has one speaker farther away from the main area and you mostly hear it coming from one direction. To remedy this, you would pan the audio such that it sounds equal.

