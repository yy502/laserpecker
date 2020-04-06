[中文测评点此处](README_CN.md)


# LaserPecker L1 & L1 Pro Review
I am a happy owner of both LaserPecker L1 and L1 Pro. Here I share some of my thoughts and uses of them. I'll refer to L1 Pro as Pro for short in the rest of the artical.


# LaserPecker
LaserPecker is brand of affordable and portable cunsumer level laser engravers. So far they have released their first generation laser engraveers (L1 and L1 Pro). The company will release more models with more powerful capabilities in 2020 and the near future.

For more details, visit their official [English site](https://www.laserpecker.net/) or [Chinese site](http://www.laserpecker.cn/).


# L1 vs L1 Pro Comparison

## The Look

![](images/L1_vs_Pro.jpg)


## Key Specifications

|  | L1 | L1 Pro |
| ------ | ------ | ------ |
| Laser | 450nm Blue, 1600mW | 405nm Blue-Violet, 500mW (equivalent to 1500mW Blue laser) |
| Pixel Size | 0.3mm (or smaller\*)| 0.15mm |
| Engrave Range|100mm x 100mm (200m x 140mm\**)| 100mm x 100mm (106mm x 106mm\*\*\*)|


\* Can be improved with an easy modification, but engraving range will reduce as a trade-off. Read on.

\*\* With Gcode. Read on.

\*\*\* With Gcode, but the improvement is so small that it's not worth the trouble.


# L1

To be updated...

# Pro

## Unpacking Pro Deluxe Edition
**What came in the Deluxe Edition**:
* Laser engraver
* USB power adapter (5V2A)
* A pair of protective Goggles
* Engraving material pack
* A 20cm ruler
* A black whiteboard marker
* A cutting mat
* USB Cables (1 long, 1 short)
* A small foldable tripod
* Automatic stand
* 4 pieces of magnetic protective shields
* A hard carry case

<img src="images/up01.jpg" height="200px"><img src="images/up02.jpg" height="200px"><img src="images/up03.jpg" height="200px">

<img src="images/up04.jpg" height="200px"><img src="images/up05.jpg" height="200px">

<img src="images/up06.jpg" height="200px"><img src="images/up07.jpg" height="200px"><img src="images/up08.jpg" height="200px">

<img src="images/up09.jpg" height="200px"><img src="images/up10.jpg" height="200px">


## LaserPecker App

Controlling the engraver is done via LaserPecker App and bluetooth over your smartphone. I do wish there's a desktop (Linux particularly) client or API available, as I'm a big fan of automation via scripting.

Don't be put off by the low rating of the App in Play Store or App Store. It isn't perfect, but it's improving and updating frequently.

There are 5 modes for image processing:
1) **Pencil**: Converts image to pencil sketch style via edge detection.
2) **G-code**: Converts image to vector paths via edge detection, mainly for cutting with (100,100) setting.
3) **Bin**: Binary, i.e. black & white mode. It converts your image to black and white for engraving.  
4) **Gray**: Converts your image to gray scale. However, the engraving results may not be as good as you expect. Material is very important. MDF boards are very good for this. Try it out for yourself. Be warned that engraving gray scale image is **very** slow, as every pixel is engraved.
5) **Seal**: Inverts your desired image/pattern for making stamps.

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

### Fabric

### Coloured Paper


### PCB (L1 vs L1 Pro)
PCB is easy to engrave. Here's a comparison of L1's and Pro's result. After the not-so-successful result of L1 at the bottom of my USB power meter (forgot about the setting), I tried my Pro on the top-left for the same texts with (30,30)x2 setting, and it looks really good. Mainly due to Pro's improved resolution.

<img src="images/pcb01.jpg" height="300px">


### PVC Sticker
Firstly, use Gcode for cutting. Secondly, cutting PVC or paper stickers will have more or less burnt edges. Instead of cutting with high power once, e.g. (100,100), using lower power setting to cut multiple times will reducing burning.

Here I used (60,50)x2. YMMV.

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

<img src="images/ps15.jpg" height="150px">




# Automatic Stand

The automatic stand was released with the Pro model. It is compatible with L1 and can be purchased separately.

Review to come...
