# All About L1 Pro (being updated...)

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


## Power Consumption & Heat Dissipation

|State|Current (mA)|
| ------ | ------ |
| Standby | 60 |
| Laser On (Adjustment) | 70 |
| Preview (marking engraving area outline) |215|
| Engraving | Up to 715|

My Pro does not run very hot. After 2 hours of continues engraving at 100% power, the engraver body was about 33°C, while the ambient temperature was 24°C. Interestingly, the fan in the stand was hotter than the engraver, at about 37°C.

<img src="images/temp01.jpg"><img src="images/temp02.jpg"><img src="images/temp03.jpg">


## Speed & Configuration

I have to say, having played with L1 before Pro, I find Pro is much slower than L1. Particularly over depth 100. So, Pro users, avoid depth 100 if you can.

I guess it's because L1's laser is more powerful, so it requires less time for the same depth.

## Precision Test

By the numbers, it is obvious that L1's precision is only 1/4 of what the Pro offers (0.3x0.3 vs 0.15x0.15). Here's how they compare with a rather extreme test image:

1) **L1 vs Pro over 100mm x 100mm**: L1 was too powerful for the paper I used. It burnt through the paper with (100,50) setting. On the other hand, Pro is less powerful and had much better control over each pixel. The slightly higher setting of (100,60) was just right for the same paper.

<img src="images/li_l1_100.jpg" height="400px"><img src="images/li_pro_100.jpg" height="400px">

2) **L1 vs Pro over 40mm x 40mm**: here you see the real difference between the two models over a much smaller job.

<img src="images/li_l1_40_3.jpg" height="400px"><img src="images/li_pro_40.jpg" height="400px">

For your interest, the source image for testing is here (click to view and download the original image):

<img src="images/lion.jpg" height="200px">


## Gcode

### Cutting

Gcode is primarily used to cut, although you can use it to engrave outlines for colouring etc. other projects and crafts.

I created a little 3D car model as below:

<img src="https://github.com/yy502/inkscape-laserpecker/misc/car.png" height="200px">

And generated [Gcode file for cutting](https://github.com/yy502/inkscape-laserpecker/misc/car.txt) using my [Inkscape extension](https://github.com/yy502/inkscape-laserpecker).

I have set to max power and slowest speed for best cutting result. If your paper is too think to cut in one go, set your LaserPecker to **cut multiple times**.


### Gray Scale

To be updated...

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

I cut up packaging boxes and engrave on the inside of the cardboard. Different types and colours of cardboard will require different settings.

<img src="images/cb03.jpg" height="200px">

### Fruit Skin

Fruit skins contain lots of water, so they require the maximum power and depth (100,100) to engrave. For Pro, depth 100 is very very very slow... Try it for yourself. The result is fun though!

<img src="images/or01.jpg" height="200px"><img src="images/or02.jpg" height="200px">


### Plastic

Plastic is easy to engrave, and you can't go too wrong about it. The only trick is that, for light coloured or clear materials, which will reflect most of the light, you need to colour it black with a whiteboard marker, so the surface will absorb laser energy. The engraved part will melt and mix with the dry ink. The rest dry ink will wipe off. See below for examples.

1.1 Colour a light-yellow plastic spoon black.

<img src="images/ko01.jpg" height="200px">

1.2 Engrave over it (30,40).

<img src="images/ko02.jpg" height="200px">

1.3 Wipe off the excessive ink, and the engraved pattern stays.

<img src="images/ko03.jpg" height="200px">

2.1 Colour a clear plastic fork black.

<img src="images/fk01.jpg" height="200px">

2.2 The result with (30,30)

<img src="images/fk02.jpg" height="200px">


3 A few more examples:

* Electric shaver case (30,30)

<img src="images/sh01.jpg" height="200px">

* Makeup bottle (30,30)

<img src="images/pl03.jpg" height="200px">

* Electric toothbrush heads (30,30)

<img src="images/pl04.jpg" height="200px">

* Water bottle (20,40) [Click here for a short video](images/pl05.mp4)

<img src="images/pl05.jpg" height="200px">

* Plastic handle of a wind-up torch (20,30)

<img src="images/pl06.jpg" height="200px">


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



# Misc

The laser does not come out from the centre of the window. It's a little to the right if you look from the front.

<img src="images/laser_head.jpg" height="250px">



# Automatic Stand

[Click Here](Auto_Stand_EN.md)