[中文评测点此处](L1_CN.md)

# All About L1

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


## Precision Test

By the numbers, it is obvious that L1's precision is only 1/4 of what the Pro offers (0.3x0.3 vs 0.15x0.15). Here's how they compare with a rather extreme test image:


1) L1 vs Pro over 100mm x 100mm

<img src="images/li_l1_100.jpg" height="300px"><img src="images/li_pro_100.jpg" height="300px">

2) L1 vs Pro over 40mm x 40mm

<img src="images/li_l1_40_3.jpg" height="300px"><img src="images/li_pro_40.jpg" height="300px">


### Now, here's some exciting stuff to see!

*L1 with magnifier modification vs Pro*

Note that:

**a)** the output of L1 was set to 100mm x 100mm, and it was scaled down to 40mm x 40mm by the magnifier;

**b)** the engraving setting for L1 with magnifier has to be reduced all the way down to (1,1) to not burn through the thick brown paper, compared to the default setting of (100,70).

<img src="images/li_l1_40_4.jpg" height="300px"><img src="images/li_pro_40.jpg" height="300px">


For your interest, the source image for testing is here:

<img src="images/lion.jpg" height="200px">


