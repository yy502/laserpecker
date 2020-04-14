[中文评测点此处](L1_CN.md)

# All About L1

L1 is cheaper, faster, slightly more powerful than the Pro. Accuracy-wise, it's not as precise as Pro. You need to think about what you want to achieve. As an owner of L1 Pro, I'd say it does not replace L1 completely, and I will keep using my L1 for certain tasks.

To be updated...

## Speed & Configuration

Having played with both L1 and Pro, I find Pro is much slower than L1. Particularly over depth 100. I guess it's because L1's laser is more powerful, so it requires less time for the same depth.

Even the default settings per material in the App are different for the two models, which is not surprising. Generally speaking, Pro's settings are slightly higher than L1's, but there's not a magic number for conversion. 


## Engraving Beyond the Designed Range

Trust me, you will love my finding!

**This trick only applies to engraving with Gcode files.**

After testing my L1 with some hand crafted Gcode, I discovered that despite the limitation of 100mm x 100mm engraving range, you can actually leverage L1's hidden X/Y axis movement capability, to engrave over as large as **200mm x 140mm** range. It's all about absolute and relative Gcode coordinates.

In short, per engraving job still has to follow the *no larger than 100mm x 100mm* rule, but each job can be placed anywhere within the 200mm x 140mm range. So, you can divide your larger vector graphics into a few small parts to be engraved one by one. I'll update my [Inkscape extension](https://github.com/yy502/inkscape-laserpecker) to simplify the generation of Gcode files for LaserPecker.

Here's a peak of the result. This was done with L1 at 20cm distance, without moving the engraver or the paper.

<img src="images/engraving_over_200mm_x_140mm.jpg" width="600px">

Video to prove it: [engraving_over_200mm_x_140mm.mp4](images/engraving_over_200mm_x_140mm.mp4)


## Cutting With Gcode

Gcode allows you to efficiently trace edges/paths. It is particularly useful for cutting materials, e.g. stickers.

### Decorative Carbon-Fibre Car Sticker

Here's an example of cutting stickers. In my test with this material, cutting once with high power is better than cutting twice with lower setting. Cutting twice resulted in more burnt edges.


<img src="images/st05.jpg" height="200px">


## Kick-Ass Modification (Cheap & Cheerful) 

Thanks to my friend **龍ARON** for sharing his simple yet amazing modification technique, it is possible to both **increases cutting power** AND **improve precision** to almost match what Pro offers. **However**, this is not a perfect upgrade to magically convert your L1 to a Pro for a few bucks. The catch is, the engraving area will reduce proportionally and significantly.

### What you will need:

1) a magnifying glass: nothing special, maybe 4x to 6x magnification (not too many times, 10x is too much). Maybe you already have one lying somewhere in your house. Its diameter should be no less than 35mm, which will cover the whole of the laser window. 50mm to 60mm diameter is ideal, purely for the easy of installation and avoid using the very edge area. Also, although a double convex lens will do the job perfectly, I recommend getting a **glass plano-convex lens** (one side is flat) if you are going to buy one for this modification, as it's easier to fix onto the engraver. It should cost around £2 if you order from Aliexpress.

This is what I used. 50mm diameter, plano-convex lens. I don't know how many time of magnification it offers, but it works as expected.

<img src="images/mod10.jpg" height="150px"><img src="images/mod11.jpg" height="150px">


2) if you have an electric stand, you don't need anything to secure the magnifier. Read on. If not, get some blue tac, or double sided tape, or simply some sellotape.


### Here's how to do it:

For those who have the electric stand, just place the lens on the stand over the laser window like so:

<img src="images/mod01.jpg" height="300px"><img src="images/mod02.jpg" height="300px">

And then, place the engraver over it and keep it up right. You may need to wedge something on the left side to keep it in the correct position.

<img src="images/mod03.jpg" height="300px">

If you do not have the electric stand, just use blue tac, or tape, to secure the magnifier on the engraver, right in front of the laser window, as close as possible.


Now, the magnifier will make the optimal focal length much shorter. It all depends on the particular magnifier you use, but it's really easy to find it.

Firstly, in the App, go to laser adjustment options and turn on the laster. It won't burn anything.

I happen to have an adjustable lab stand that's perfect for the job. You can just get a piece of paper, and use a stack of objects (books, building blocks, Lego, etc.) to gradually raise the paper towards the engraver while observing the laser dot **with your protective goggles on** to reduce from a short line to a fine dot. In my case, the new focal length is 9cm.

<img src="images/mod04.jpg" height="280px"><img src="images/mod05.jpg" height="280px"><img src="images/mod06.jpg" height="280px"><img src="images/mod07.jpg" height="280px">


Now, very important, exit the laser adjustment mode, and engrave something that's easy to measure. e.g. a 10cm circle or box. And then measure the output size.

In my case, each axis has reduced to 40% of the output size. i.e. a 100mm circle becomes 40mm. Which means, the **max** engraving area is now only **40mm x 40mm**. So, if you want to engrave an image of which longest side is 30mm, you need to set it to 30/0.4=75mm in the App.

<img src="images/mod08.jpg" height="300px"><img src="images/mod09.jpg" height="300px">


Do not get upset yet, here's what you have **gained**:

1) the laser dot now is much smaller than the original 0.3mm x 0.3mm one, meaning the precision is close to Pro's 0.15mm x 0.15mm. *Read the next section for some exciting comparison!*

2) because the power is unchanged but the laser dot is now smaller, the relative power over the smaller dot is much higher. Now your L1 can cut through materials that it could not even engrave on! e.g. my L1 with a magnifier was able to cut standard white address sticker labels, which my L1 without the modification could not even leave a mark on it.

Here's a test cut on a thick cardboard.

<img src="images/mod12.jpg" height="300px"><img src="images/mod13.jpg" height="300px">

So, with this mod, you don't really need a Pro to achieve high precision engraving, if you only need to engrave over small areas ;-)



## Precision Test

By the numbers, it is obvious that L1's precision is only 1/4 of what the Pro offers (0.3x0.3 vs 0.15x0.15). Here's how they compare with a rather extreme test image:

1) **L1 vs Pro over 100mm x 100mm**: L1 was too powerful for the paper I used. It burnt through the paper with (100,50) setting. On the other hand, Pro is less powerful and had much better control over each pixel. The slightly higher setting of (100,60) was just right for the same paper.

<img src="images/li_l1_100.jpg" height="400px"><img src="images/li_pro_100.jpg" height="400px">

2) **L1 vs Pro over 40mm x 40mm**: here you see the real difference between the two models over a much smaller job.

<img src="images/li_l1_40_3.jpg" height="400px"><img src="images/li_pro_40.jpg" height="400px">

For your interest, the source image for testing is here (click to view and download the original image):

<img src="images/lion.jpg" height="200px">


### Now, here's some exciting stuff to see!

*L1 with magnifier modification vs Pro*

Note that:

1) the output of L1 was set to 100mm x 100mm, and it was scaled down to 40mm x 40mm by the magnifier;

2) the engraving setting for L1 with magnifier has to be reduced all the way down to (1,1) to not burn through the thick brown paper, compared to the default setting of (100,70).

<img src="images/li_l1_40_4.jpg" height="400px"><img src="images/li_pro_40.jpg" height="400px">



