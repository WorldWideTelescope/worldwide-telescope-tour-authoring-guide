+++
title = "Dealing with Audio"
weight = 500
+++

AAS WorldWide Telescope can play back a separate stereo voice-over and music
tracks to tell a narrative story and provide a music soundscape for a tour.


# Strategies

WWT can play a variety of audio files. Playback quality is limited to the
quality of the input audio file so start with the highest quality. If you are
getting an existing file or if you are creating your own try to get a lossless
format, like WAV, or a high-bitrate one, like 320 kbps MP3.

Before starting to create audio you should decide which of two general
strategies you want to follow. The first is to produce an entire audio file
for the entire tour and the other is to create separate audio files that are
tied to each slide. The advantage of creating a single audio file is that you
can globally adjust the level for audio on all slides, and work on global
timing. However, for narration you will have to acquire a long sequence in one
go, or use an audio editor to cut out sections, replace flubs etc. Also, if
audio is recorded as one long track and you change the timing of the visuals
you have to re-record or re-edit the narration track.

For these reasons, the recommended way to do audio is to place the musical bed
as a single soundtrack and to include narration audio on a per-slide basic.
This how-to will show how to do this.

1. Get at least a draft of your tour done visually. Words drive the visuals and
   visuals drive the audio. The visuals will also provide an estimate of the tour
   length.
2. Find an audio file that has the sound and length that fit your tour —
   nowadays there are many sources of free, reusable music online.
   Ambient-style music is more appropriate to loop and thus allows a shorter
   file to be used as a bed for a longer tour.
3. Make a short first slide. I often make the tour and then duplicate the
   first slide and make the first of the duplicates a very short – 0.5 to 1.0
   second – slide. Make this slide a Master and don’t have any – or a very
   small amount of – motion and don’t have any text or images. The reason we
   make a short Master is to separate audio that spans multiple slides from
   text and images that will be on only a slide or two. If you put these
   elements onto a Master slide they will persist until the next master slide.
4. Add the audio to the slide buy clicking on Browse under Music in the upper
   right hand of the WWT window. Browse to the music file. You can enter a
   Fade In and Fade Out times for the music and setting it to automatically
   repeat or not. Adjust the slider to be 1/2 to 2/3 the way to maximum. Since
   this is a Master slide, the music will play over all slides until the tour
   hits a music track on another Master slide.
5. You can add music tracks on a per-slide basis which will be mixed into the
   musical bed of the master slide. This might be useful if you wanted to
   coordinate a sound effect coordinated with a visual on one slide.
6. Assuming you have a script, which may or may not be displayed as text on
   each slide, you know what words to say for each slide. Record a voiceover
   file (e.g., MP3) for each slide. It is worthwhile to label the slides with
   text and use the automatic slide numbering (check Guided Tours/Show Slide
   Numbers) for the slides and use a similar naming for the narration audio
   files. When recording try to use a quiet room without hard surfaces (i.e.,
   carpet, drapes and objects in the room are good and fans air conditioners
   etc. are bad). It is useful to normalize the voiceovers in their
   uncompressed form before compressing to MP3. You want to make sure that the
   slide is at least as long as the narration audio. Add the audio by clicking
   Browse for Voiceover which is just below the Music selector.
7. You can preview the tour from that slide and adjust the level of the
   narration relative to the music. When in doubt it is more important to be
   able to hear the voiceover than the music.


# Editing Audio

Here we illustrate how to edit audio using an open source windows program
called [Audacity](http://audacity.sourceforge.net/). Most audio editing
software can probably do the same things.

I edit audio for the following purposes: trimming, normalization, background
noise removal, and format conversion. I would do all editing in WAV and then
convert to MP3 at the last step. Also, I would use draft audio until you have
finalized the visual timing and then do audio editing and conversion.

## Trimming

When you get music of narration files often the timing of the files needs to
be adjusted. When you know the timing of the tour you are trying to match and
the audio file you may need to cut some off of the audio file. Cutting the
length for the file can make is smaller and you can also add custom fades (in
and out) at this point.

Figure out the time you want to trim to and if you want to add a fade in or
fade out. For this example I will put a 2 second fade out at the end of a
musical audio file. Since the music builds gradually, I will not change the
beginning of that with a fade-in.

1. Open Audacity and load input audio file. Identify the length you want the
   audio piece to be.
2. Use mouse to select 2 seconds from the end.
3. Click “Effect” in the top menu and select “Fade Out.” This will create a
   linear fade out that you can see graph in Audacity.
4. Select from the beginning to the end of the ending fade.
5. Click “File” in menu and “Export Selection.”
6. Choose WAV — assuming you will save this uncompressed WAV file as an
   archive and convert to MP3 in another step (see below).

## Normalization

Audio is inherently analog and capturing a digital copy requires you to sample
it into a range of digital values. Digitized signals have specific steps
between each level. In order to have the best sounding signal it should be
normalized such that the maximum signal is at the highest value of the digital
signal. This has the effect of making the signal as loud as it can be without
clipping. Then you can reduce the volume with the slider in WWT.

1. Open Audacity and load input audio file. Identify the length you want the
   audio piece to be.
2. Use mouse to select the entire file (or the part you want to export and
   use).
3. Click “Effect” in the top menu and select “Normalize.” This will bring up a
   dialog box. I check all boxes and set the maximum amplitude to 0.0 dB. This
   will scan the file and determine the scaling to amplify the signal to the
   maximum values.
4. Select from entire file of a selection.
5. Click “File” in menu and “Export Selection.”
6. Choose WAV — assuming you will save this uncompressed WAV file as an
   archive and convert to MP3 in another step (see below).

## Background Noise Removal

1. Open Audacity and load input audio file.
2. Put cursor in file window and select a part of the audio file where there
   is noise. You may want to expand the range to see this clearly.
3. Click “Effect” in the top menu and select “Noise Removal …” This will bring
   up a dialog box. Click “Get Profile.”
4. Then select the entire audio file (or the part you want to save out).
5. Click “Effect” in the top menu and select “Noise Removal …” This will bring
   up a dialog box. I leave the default values and then make sure “Remove” is
   selected and click the “OK” button.
6. Click “File” in menu and “Export Selection.”
7. Choose WAV — assuming you will save this uncompressed WAV file as an
   archive and convert to MP3 in another step (see below).

## Format Conversion

If you are getting music files, WAV files are great for quality, but can be
large. Note, that tours encapsulate assets like audio and images so be aware
that file sizes could be large if you include uncompressed audio like WAV. I
suggest working with WAV files and keeping copies of those around for editing,
but before putting the files into WWT, converting it to compressed MP3.
Audacity can read in almost any format file and you can select the same file
for export to another format.

1. Open Audacity and load input audio file.
2. Put cursor in file window and Control-A (select all).
3. Under “File” click “Export Selection.”
4. In the dialog box that comes up, select “MP3 Files” as output format.
5. Click the “Options” button which opens a box to select MP3 output encoding
   options. I use Variable Bit Rate, Quality level 5, 110-150 kbps. You can
   also use Constant Bit Rate with 128 kbps or higher.
6. Load the file into WWT and play it back to make sure it sounds ok. If you
   are in a very quiet room with good acoustics and speakers you might hear
   MP3 compression and want to use a higher bit rate. Note that variable bit
   rate MP3 use file space a bit more efficiently and plays fine in WWT.
