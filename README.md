## Thomann Stompenberg Dataset

This dataset has been generated using https://www.thomann.de/gb/stompenberg_devices.html
using whatever device in bypass mode and with speaker simulation disabled.

### Single tracks

All files are pcm_f32le 48000

Files has been recorded in mono from browser using Audacity with pulse device and pulse volume control control panel.
Both bass and guitar tracks have been recorded with the same volume levels for all the recording session.
The following processing has been applied:
- trim silence selecting the start -40dB duration 0.1s compress 5%
- trim silence selecting the end -40dB duration 0.1s compress 5%

Then the tracks has been exported as WAV float32 48000.

NOTE: some files may have < 0.1s of silence at beginning, so the trim silence command
took no effect

Audacity project was set to 48000.

### Full mix

A single file with all the tracks concatenated has been created since
is often preferred during training. For such scope two format are provided:
- pcm_f32le 48000
- pcm_s16le_44100
For 44100 export track has been resampled by Audacity.
Full mix has been normalized to -6dB peak + DC offset removal before export.

### Instrument mixes

A separated mix for each instrument (guitar, bass) has been created in the following
formats:
- pcm_f32le 48000
- pcm_s16le_44100
For 44100 export track has been resampled by Audacity.
No normalization has been applied to instrument mixes

### License

This data set has been created for research purposes and is available under

the Creative Commons Attribution-ShareAlike 4.0 International License ("by-sa")
