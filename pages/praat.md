---
layout: default
title: Praat 
nav_order: 3
permalink: praat
---
# Working with Praat
## Loading sound files
Once Praat is installed, you can open the software from the Applications folder. Two windows will open: one for the Praat objects and one for the Praat picture. The objects window is where you will load and manipulate sound files. You can close the picture window as it is not necessary for the pipeline.

In the Praat Objects window, open the MP3 file by going to the top left of the screen and select:
* Open → Read from file
* Navigate to the `ETC_private` folder and select the MP3 files you want to process.

Example path: 
```
/ETC_Private/Assessment_Speech/Data/ETC05/ETC05_L_24mo
```

Select as many files as you want to process. You can select multiple files by holding down the `shift` key and clicking on the files you want to process. Once you have selected the files, click `Open`. The files will load into the Praat Objects window.

Once the files are loaded, select all of the files by clicking on the first file, holding down the `shift` key, and clicking on the last file. 

Then, go to the right side of the screen and select `Annotation` → `To TextGrid`. This will create a TextGrid for each sound file.

A window will pop up asking you to specify tier names and point tiers. You must delete the default value for `All tier names` to `window` and leave `Which of these are point tiers?` empty. Then click `OK`.

{: .note }
`window` is the only tier name that will work with the pipeline. If you use a different tier name, the pipeline will not work. Changing tier names is challenging, so it is best to make sure you type `window` from the start.

<img src="{{ site.baseurl }}/img/praat-settings.png" alt="im" width="400"/>

## Creating TextGrids
Once the TextGrids are created, you will see a new file for each audio recording in the Praat Objects window. You want to select both the sound file and the TextGrid file for each recording. You can do this by holding down the `shift` key and clicking on the 2 files you want to select. Make sure that the sound file and the TextGrid file have the same name. A good way to check is to look at the configuration number in the file name. This will be a number between 00 and 15 and is located right after the timepoint (e.g., `12mo_04`). If the sound file is `ETC07_R_12mo_07_5_0mA`, the TextGrid file should be the same.

<img src="{{ site.baseurl }}/img/praat-both-selected.png" alt="im" width="400"/>

With both files selected, go to the right side and select View & Edit. This will open a new window with the sound file and the TextGrid file. 

## Viewing the files
The top two windows are audio file modules; the top window shows the waveform and the middle window shows the spectrogram. You will need to zoom in further to view the spectogram. 

The TextGrid file is located in the bottom window. Off to the right you will see letters and symbols (not shown in screenshot). You can ignore these. 

<img src="{{ site.baseurl }}/img/praat-layout.png" alt="im">

The waveform is helpful for seeing when the syllable begins and ends because it goes from a flat line to a wave and vice versa.

This tool shows the [formants](http://www.phys.unsw.edu.au/jw/formant.html), with the blue line indicating the base formant. Each formant corresponds to a resonance of the vocal tract(frequency at which the vocal folds are vibrating). The formants run horizontality, but when stacked, they look like dark black bands running vertically from the top to the bottom of the spectrogram window.

## Playing the audio file
Click on the left-hand side of the wave in the top window to move the red cursor line. Then click `tab`. This will play everything to the right of the cursor that is in the playable window.

To listen to a specific part of the audio file, click and drag the mouse over the waveform. Then click `tab` to play the selected portion.

There should be roughly 10 of each syllable, but listen to the recording to
make sure you are analyzing the correct syllables.

## Defining the windows
Each TextGrid should be divided into 7 windows. The order of the windows is as follows:
1. Cushion
2. Vowels (ka/)
3. Cushion
4. Vowels (ta/)
5. Cushion
6. Vowels (pa/)
7. Cushion

The order could vary if the syllables are not recited in the order ka/ta/pa/. This will not affect the pipeline.


{: .note }
The pipeline will not work if there is not a window after pa/. It's okay if this window is very short, but it must be present.

The three vowel windows should include all repetitions of each syllable. It is recommended to include a few milliseconds of silence before and after the syllable. This will help the pipeline identify the syllable. 

The silence or background noise windows should cushion the vowel windows. There should be at least 4 of these windows. 

Avoid overlapping windows. If you have overlapping windows, the pipeline will not work.

To define the windows, click on the waveform and drag the mouse to the right. This will define a window. If the window is too large or too small, click outside of the window and define a new area. To save the window, click  `Interval` → `New interval on tier 1`.

<img src="{{ site.baseurl }}/img/praat-add-int.png" alt="" width="400">

Once all the windows are defined, select each syllable interval and type either k, t, or p. This will label the interval with the corresponding syllable. Leave the cushion intervals blank.

Below is a screenshot of what the TextGrid should look like when it is complete. Check that in the bottom left you see `window (#/7)`.

<img src="{{ site.baseurl }}/img/praat-final.png" alt="A screenshot of a completed TextGrid file">
