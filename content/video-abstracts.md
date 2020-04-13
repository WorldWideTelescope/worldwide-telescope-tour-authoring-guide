+++
title = "Sample Workflow: Video Abstracts"
weight = 700
+++

This section walks through a workflow that you might use to prepare a WWT tour
that can act as a “video abstract” to a scientific paper.


# Video Tutorial

{{ youtube(id="6SA-VJUb3w0", class="youtube-embed") }}


# Preliminaries

The first question to ask yourself is: can one or more images be used as a
primary way to communicate the main science result?

If the answer is no, it will be difficult to make a video abstract completely
with WWT. It will take more time and WWT could be used for parts, but final
abstract would have most of the visuals created outside of WWT and edited
together.

If yes, keep reading.


# Time Budget

We estimate the total time to make such an abstract to be about 6–14 hr:

1. Prepare data: 0–4 hr
2. Make storyboard: 0.5 hr
3. Write draft script: 1 hr
4. Record draft narration: 0.5 hr
5. Create draft tour: 1–3 hr
6. Create draft video (optional): 0.5 hr
7. Gather feedback: 1.0 hr (not including waiting for other people to get back
   to you!)
8. Record final narration: 0.5–1.5 hr
9. Refine tour: 1–2 hr
10. Create final video (optional): 0.5 hr


# Step 1: Prepare data

Some abstracts can be presented with the data in WWT, adding only text and
image overlays. Other, more complex tours will want to represent the original
new data presented in the paper. In these cases, significant time might have
to be taken to import FITS or other data formats into WWT.

Below is one representative workflow used to get the data into WWT necessary
for a video abstract. This workflow assumes that the data that will be added
to WWT in order to present the abstract are in the form of FITS files.

1. Use [FITS Liberator] to make a TIFF from original FITS file.
   1. Had to select "No Flip" (which controls vertical flips)
   2. The image was still flipped horizontally, so …
   3. Loaded output TIFF into Photoshop and did a horizontal flip and resaved
2. Test by loading large TIFF into WWT
3. When final TIFFs are made, publish them online somewhere.
4. Import the image into WWT using
   [the ImportImage tool](http://worldwidetelescope.org/GetInvolved/ImportImage).
5. Download the
   [collection (WTML) file](https://docs.worldwidetelescope.org/data-guide/1/data-file-formats/collections/)
   which has reference to new tiled images that can now be used in a tour.

[FITS Liberator]: https://www.spacetelescope.org/projects/fits_liberator/

In the example, this was done for two images. One was the astronomical VLA
image `Sgr_A_West-Ka` and the second was a line plot. For the plot, the
coordinates were copied from an image at the same scale. The plot was exported
from Illustrator as a PNG with transparency everywhere except where the lines
of the plot were to be drawn.

Many different kinds of data can be imported and rendered within WWT, as
described in the [Layer Guide] and [Data Guide].

[Layer Guide]: https://docs.worldwidetelescope.org/layer-guide/1/
[Data Guide]: https://docs.worldwidetelescope.org/data-guide/1/


# Step 2: Make storyboard

The storyboard is a sequence of draft visuals representing what will be on
screen. It can be in the form of descriptions of what is to be shown or a list
of figures (from WWT as well as those in the paper). In the case of the
example Proplyd paper, it was a list of figures, selecting those from the
paper that directly supporting the words of the written abstract (script of
the tour).


# Step 3: Write draft script

Drafting a script in either bullet or written form is the first step in the
process. The simplest way to do this is to read the written abstract with
modest revisions for acronyms, jargon and detailed numerical data. In an
example, reading the text of the abstract verbatim took about 2:15.


# Step 4: Record draft narration

Record draft narration for timing. Don’t worry about flubs or mistakes as long
as they don’t change the time appreciably. It is suggested to use
[Audacity](https://audacity.sourceforge.net), which is a free tool available
on Mac OS, Linux or Windows to record and edit audio. However, feel free to
use any program that can create a high-quality MP3 file. See the
[Audio](@/audio.md) section for further advice.


# Step 5: Create draft tour

Create a draft tour showing visuals timed to draft narration. Note that there
are two type of tours. The simplest is a “slide-based tour” which is composed
of a sequence of slides, each with a begin and end position. The
visualizations are interpolated between the beginning and end of each slide.
Slide-based tours can be played back in the web tour player or the Windows
Desktop client.

There is a more advanced type of tour called a timeline, or keyframe-based,
tour. Timeline tours provide fine-grained control over the tour with the
ability to specify any parameter at any time (down to 1/30 of a second).
Timeline tours can provide more cinematic tours but cannot currently be played
back in the web tour player and can only be shared on-line in the form of
videos. Since much of the power of WWT-based video abstracts comes from
comparing data supporting the journal article with other data, you should
create your tour as a slide-based tour. After this is created for your paper,
you can convert a slide-based tour into a timeline one in order to make a more
polished video but the tour directly related to your paper would be the
slide-based, web-playable version.

When you are finished with the tour, make sure to save your tours with good
naming and versioning information to help organize your files as you refine in
the later steps.


# Step 6: Create draft video (optional)

You have to use the WWT Windows client to render the tour to a sequence of
image frames. Instructions on that are available in the
[Rendering to Video](@/render-video/index.md) section.

Once you have the frames, you need to use a program to take that and the audio
narration and encode them as a video. This is straightforward to do with a
modern video encoder, such as Adobe Premiere. It is also possible to use the
cheap Apple QuickTime program to do this. This process may take a while to
complete, but user interaction time is modest. When complete, you will likely
want to post your video YouTube or similar video sharing service to share with
your colleagues for feedback.


# Step 7: Gather Feedback

Share your tour with colleagues (e.g., co-authors on paper) to get feedback.
Sharing the tour can be done in one of a few ways:

1. If they have a Windows PC with WWT installed, you can share the tour file
   itself, which should be small unless you have many high-resolution images
   included.
2. You can also share the YouTube video link if you did the optional step of
   making a video from the tour (see Section 6 above). This of course can be
   viewed on most desktop and mobile devices.
3. You can also share a link to the web client. **TODO more details**.

Organize the responses and make clear choices about what you will change to
address them. This is likely to be in form that you assumed the viewer would
know something and need to add descriptive text on screen or in narration for
those that don’t. This will likely require changes to the script as well as
tour (timing and adding text labels, data etc.).


# Step 8: Record final narration

Refine script and record new audio based on feedback. You will use the same
tools as you did to record the draft narration. However, you will want to get
a high a quality recording as possible (good microphone, quiet room, a fresh
voice). You may want to embellish the narration with a music or ambient sound
bed. If you do add music, make sure that is low in volume, compared to the
narration.


# Step 9: Refine tour

Refine tour based on feedback. Use the final audio for final timings. Slide
lengths may need be changed to accommodate changes in narration timing. Also


# Step 10: Create final video (optional)

Using the same work flow as you did to create the draft video, create the
final one. The steps are essentially the same.
