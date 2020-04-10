[中文测评点此处](README_CN.md)

# LaserPecker L1 & L1 Pro Review
I am a happy owner of both LaserPecker L1 and L1 Pro. Here I share some of my thoughts and uses of them. I may refer to L1 Pro as Pro for short in the rest of the article.


# LaserPecker
LaserPecker is brand of affordable and portable consumer level laser engravers. So far they have released their first generation laser engravers (L1 and L1 Pro). The company will release more models with more powerful capabilities in 2020 and the near future.

For more details, visit their official [English site](https://www.laserpecker.net/) or [Chinese site](http://www.laserpecker.cn/).


# L1 vs L1 Pro Comparison

## The Look
L1 and Pro are of the same size & design, with minor difference as shown below. Therefore both will fit onto the automatic stand. 

![](images/L1_vs_Pro.jpg)


## Key Specifications

|  | L1 | L1 Pro |
| ------ | ------ | ------ |
| Laser | 450nm Blue, 1600mW | 405nm Blue-Violet, 500mW (equivalent to 1500mW Blue laser) |
| Pixel Size | 0.3mm (or smaller\*)| 0.15mm |
| Engrave Range|100mm x 100mm (or larger\**)| 100mm x 100mm (106mm x 106mm\*\*\*)|


\* Can be improved with an easy modification, but engraving range will reduce as a trade-off. Read on.

\*\* With Gcode. Read on.

\*\*\* With Gcode, but the improvement is so small that it's not worth the trouble.


# L1

L1 is cheaper, faster, slightly more powerful than the Pro. Accuracy-wise, it's not as precise as Pro. You need to think about what you want to achieve. As an owner of L1 Pro, I'd say it does not replace L1 completely, and I will keep using my L1 for certain tasks.

To be updated...

## Engraving Beyond the Designed Range
Trust me, you will love my finding!

**This trick only applies to engraving with Gcode files.**

After testing my L1 with some hand crafted Gcode, I discovered that despite the limitation of 100mm x 100mm engraving range, you can actually leverage L1's hidden X/Y axis movement capability, to engrave over as large as **200mm x 140mm** range. It's all about absolute and relative Gcode coordinates.

In short, per engraving job still has to follow the *no larger than 100mm x 100mm* rule, but each job can be placed anywhere within the 200mm x 140mm range. So, you can divide your larger vector graphics into a few small parts to be engraved one by one. I'll update my [Inkscape extension](https://github.com/yy502/inkscape-laserpecker) to simplify the generation of Gcode files for LaserPecker.

Here's a peak of the result. This was done with L1 at 20cm distance, without moving the engraver or the paper.

<img src="images/engraving_over_200mm_x_140mm.jpg" width="600px">

Video to prove it: [engraving_over_200mm_x_140mm.mp4](images/engraving_over_200mm_x_140mm.mp4)


## Kick-Ass Modification (Cheap & Cheerful) 

Hint: increases cutting power, improves resolution to (almost) match Pro's

To be updated...




# Pro

## Unpacking Pro Deluxe Edition
**What came in the Deluxe Edition**:
* L1 Pro laser engraver
* USB power adapter (5V2A, US/CN plug)
* Engraving material pack
* A 20cm ruler (for measuring the optimal distance for engraver placement)
* A black whiteboard marker
* A cutting mat
* USB Cables (1 long, 1 short)
* A small foldable tripod
* Automatic stand
* A pair of protective goggles (filters harmful laser light)
* 4 pieces of magnetic protective shields (filters harmful laser light)
* A hard carry case

<img src="images/up01.jpg" height="200px"><img src="images/up02.jpg" height="200px"><img src="images/up03.jpg" height="200px">

<img src="images/up04.jpg" height="200px"><img src="images/up05.jpg" height="200px">

<img src="images/up06.jpg" height="200px"><img src="images/up07.jpg" height="200px"><img src="images/up08.jpg" height="200px">

<img src="images/up09.jpg" height="200px"><img src="images/up10.jpg" height="200px">


## LaserPecker App

Controlling the engraver is done via LaserPecker App in your smartphone over Bluetooth. I do wish there's a desktop (Linux particularly) client or API available, as I'm a big fan of automation via scripting.

Don't be put off by the low rating of the App in Play Store or App Store. It isn't perfect, but it's improving and updating frequently.

There are 5 modes for image processing:
1) **Pencil**: Converts image to pencil sketch style via edge detection.
2) **G-code**: Converts image to vector paths via edge detection, mainly for cutting with (100,100) setting.
3) **Bin**: Binary, i.e. black & white mode. It converts your image to black and white for engraving.  
4) **Gray**: Converts your image to gray scale. However, the engraving results may not be as good as you expect. Material is very important. MDF boards are very good for this. Try it out for yourself. Be warned that engraving gray scale image is **very** slow, as every pixel is engraved.
5) **Seal**: Inverts your desired image/pattern for making stamps.

Known bug (Android): if the App has connected to the engraver, and you hit Back button a few times to get back to the initial page before choosing an engraver to connect to; and then try to search for the engraver, the App won't find any. You will need to force kill the App, and the relaunch it to start over. A little annoying, but it's not the end of the world.


## Power Consumption & Heat Dissipation

## Speed & Configuration

## Accuracy Test

## Manipulation via Gcode

### Gray Scale & Cutting

## Working with Different Materials

Throughout my article, I will use the notation of (P,D)xT to indicate the engraving configuration, where P is power, D is depth and T is times of engraving. I will omit x1 time, so (100,80)x1 becomes (100,80), meaning power:100, depth:80, once. (50,20)x2 means power:50, depth:20, 2 times. (30,50)x3 means power:30, depth:50, 3 times.

Remember, the engraving configurations for different materials in the App are only recommended values. Apart from material, colour, density and even room temperature will have some impact on the result. So I suggest you either do some test engraving before your "big job", or start with low power, shallow burns and work your way up to avoid over burning your material.

Sometimes, multiple low power shallow burns are better than one hig power deep burn. For example, I prefer using 80,50 x2 times in Gcode mode to cut PVC stickers, rather than using 100,80 to cut once. The edges are much better (less burnt).

The bottom lines is, there's no perfect setting for a class of materials. Don't get frustrated or upset when you fail to achieve what you wanted in one go. The more you play with your LaserPecker, the better you will know its capabilities and performance on different materials. Do take notes of the perfect configurations that you have tested out for specific materials which you frequently use.


### Wood
Wood is one of the most easy & satisfying materials to engrave. Darker wood grain is harder to burn in, while lighter wood grain can be engraved with lower power. So, for relatively consistent result, I suggest you over-burn a little. For this dark wood of mine, I used (100,80). Again, don't just take my settings. Do some test burns by yourself and find the best setting for your material.

**Tip**: If the first go leaves an uneven result. Do not touch your material and do a 2nd burn over it with the same or higher setting.

<img src="images/w01.jpg" height="200px"><img src="images/w02.jpg" height="200px">

### Cardboard

### Plastic

Plastic is easy to engrave, and you can't go too wrong about it. The only trick is that, for light coloured or clear materials, which will reflect most of the light, you need to colour it black with a whiteboard marker, so the surface will absorb laser energy. The engraved part will melt and mix with the dry ink. The rest dry ink will wipe off. See below for examples.

1.1 Colour a light-yellow plastic spoon black.

<img src="images/ko01.jpg" height="200px">

1.2 Engrave over it (30,40.)

<img src="images/ko02.jpg" height="200px">

1.3 Wipe off the excessive ink, and the engraved pattern stays.

<img src="images/ko03.jpg" height="200px">

2.1 Colour a clear plastic fork black.

<img src="images/fk01.jpg" height="200px">

2.2 The result with (30,30)

<img src="images/fk02.jpg" height="200px">


3.1 Another example: electric shaver case (30,30)

<img src="images/sh01.jpg" height="200px">


### Eyeglass Cleaning Cloths

I find the default (100,70) for cloths does not work well with microfiber cloths, maybe it's for cotton cloths. I reduced it to (100,50) and got satisfying result. See below for comparison.

<img src="images/cl01.jpg" height="200px">


### Coloured Paper


### PCB (L1 vs L1 Pro)
PCB is easy to engrave. Here's a comparison of L1's and Pro's result. After the not-so-successful result of L1 at the bottom of my USB power meter (forgot about the setting), I tried my Pro on the top-left for the same texts with (30,30)x2 setting, and it looks really good. Mainly due to Pro's improved resolution.

<img src="images/pcb01.jpg" height="300px">


### Decorative Carbon-Fibre Car Sticker
Firstly, please use Gcode mode for cutting.

Secondly, cutting plastic or paper stickers will have more or less burnt edges. Instead of cutting with high power once, e.g. (100,100), using lower power setting to cut multiple times will reducing burning.

Here I used (60,50)x2. YMMV. Remember that colour plays a role here, too.

<img src="images/st01.jpg" height="200px"><img src="images/st02.jpg" height="200px">

<img src="images/st03.jpg" height="200px"><img src="images/st04.jpg" height="200px">


### Felt Paper
I have cut these for my son to play with. Instead of (100,80), I used (80,60)x2 in Gcode mode for a clean cut. Occasionally, I had to use utility knife to cut part of the shape off.

<img src="images/fp01.jpg" height="160px"><img src="images/fp02.jpg" height="160px"><img src="images/fp03.jpg" height="160px"><img src="images/fp04.jpg" height="160px"><img src="images/fp05.jpg" height="160px"><img src="images/fp06.jpg" height="160px"><img src="images/fp07.jpg" height="160px"><img src="images/fp08.jpg" height="160px"><img src="images/fp09.jpg" height="160px"><img src="images/fp10.jpg" height="160px"><img src="images/fp11.jpg" height="160px"><img src="images/fp12.jpg" height="160px"><img src="images/fp13.jpg" height="160px"><img src="images/fp14.jpg" height="160px"><img src="images/fp15.jpg" height="160px"><img src="images/fp16.jpg" height="160px"><img src="images/fp17.jpg" height="160px"><img src="images/fp18.jpg" height="160px"><img src="images/fp19.jpg" height="160px"><img src="images/fp20.jpg" height="160px"><img src="images/fp21.jpg" height="160px">


### Photosensitive Stamp

The App's Seal mode will do the inversions for you. All you need to do is to design what your stamp should look like, and engrave the image in the App's Seal mode. The part that is engraved will melt and seal up, meaning it won't absorb ink or let ink out. The unprocessed part of the photosensitive stamp will absorb ink and make a mark on paper.

Here are two styles of stamps that I made. In Chinese, these are called Yin and Yang engraving.

**Stamp 1: Yin Engraving** (5,75)

<img src="images/ps21.jpg" height="160px"><img src="images/ps22.jpg" height="160px"><img src="images/ps23.jpg" height="160px"><img src="images/ps24.jpg" height="160px">

The design on the plastic cover with (30,30).

<img src="images/ps25.jpg" height="160px">

**Stamp 2: Yang Engraving** (5,75)

<img src="images/ps11.jpg" height="160px"><img src="images/ps12.jpg" height="160px"><img src="images/ps13.jpg" height="160px"><img src="images/ps14.jpg" height="160px">

The design on the plastic cover with (30,30).

<img src="images/ps15.jpg" height="160px">




# Automatic Stand

The automatic stand was released with the Pro model. It is compatible with L1 and can be purchased separately.

The stand folds up and fits into the carry case nicely. It does not have built-in battery. You will need one USB C cable to feed power to it; and it relays the power to the engraver via another short USB C cable. Both cables come along with the stand.

I have put a carbon-fibre sticker onto the base, and engraved a 100mm x 100mm grid over it to assist alignment of target objects. The grid is done via Gcode. I actually has 3 designs of the grids in Gcode files which can be found here: [yy502/inkscape-laserpecker/](https://github.com/yy502/inkscape-laserpecker/) in `misc` directory. 

<img src="images/es01.jpg" height="200px">
<img src="images/es02.jpg" height="200px">
<img src="images/es03.jpg" height="200px">
<img src="images/es04.jpg" height="200px">
<img src="images/es05.jpg" height="200px">
<img src="images/es06.jpg" height="200px">