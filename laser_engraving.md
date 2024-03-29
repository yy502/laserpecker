# Laser Engraving Tips & Tricks

## Safety

moved to https://lp.systemd.one/?p=266


## Baking Soda Magic (on wood and fabric)

moved to https://lp.systemd.one/?p=270


## Dithering

Dithering an image means to use different densities of black and white pixels to emulate grayscale. The end goal is to use Bin mode (B&W) to engrave (or print) something that appears in grayscale.

### Step 1 - Resize

You **must** firstly decide your engraving size (e.g. 60mm x 40mm), and use your engraver's output resolution (pixels per mm) to work out the optimal size of the image in pixels. For L1/Pro, the engraving resolution is 10px/mm. For LP2, choose from 10px/mm (1k), 13px/mm (1.3k) or 20px/mm (2k) and stick with it.

Use `size (mm) x resolution (px/mm)` to get image size in pixels. Ignore dpi if you see it in your image resize tool. it's just another representation/unit of resolution. 10px/mm = 254dpi, 13px/mm = 330dpi and 20px/mm = 508dpi if you must know.

For example, I want a 60mm x 40mm engraving in 10px/mm resolution, I want to resize my image to 60x10=600px by 40x10=400px. If I use 2k resolution with my LP2, and I want an engraving of 50mm x 10mm, the optimal image size is 50x20=1000px by 10x20=200px.

The reason why it's so important to resize the image and stick with the output size is to avoid having the App to resize (scale down) the image for engraving, and produce **scaling artifacts**, which will look like some ghosting grid or rings in your engraving, but not visible in your converted image. It is a **mathamatical problem** (sampling), not a hardware issue. You can observe this by slowly zooming in and out a dithered image on your phone. Here is some additional info about it: http://www.glennchan.info/broadcast-monitors/scaling-artifacts/scaling-artifacts.htm

### Step 2 - Dither

A popular free & powerful browser-based tool is [imag-r.com](imag-r.com). You simply upload your image, resize it (there's a reason why the tool wants you to resize the image as step-1, see above!), and select a suitable profile to dither it. Finally downlaod the dithered image and send to LP App for engraving. I recommand you write the resolution and output size in mm in the file name if you want to reuse the dithered images.

Another tool is the built-in **Newsprint** filter of [GIMP](https://www.gimp.org/). Try different patterns (lines, dots, dimands, etc.), angle and sampling settings. Again, you need to resize your image first. Here's an example of a dog engraved on a Post-It note in Bin mode (ignore the gaps in the engraving, I accidentaly moved the paper during engraving):

<img src="images/np01.jpg" height="600px"><img src="images/np04.jpg" height="600px">

<img src="images/np02.jpg" height="300px"><img src="images/np03.jpg" height="300px">

### Step 3 - Engrave

Engrave in **Bin** mode, NOT Gray. That's the whole point of dithering.

Remember to stick with your initial choices of engraving size (and resolution if using LP2).

If you want to engrave it in a different size, re-dither your source image from the beginning.

## Glass work (L1/Pro)
moved to https://lp.systemd.one/?p=382

## Image Correction Tool for Engraving Conical Objects (LP2 + 3rd Axis)
http://laserpecker.systemd.one/image_converter.html
