# Know Your LP3

## LP2 vs LP3 (including the upgraded stand)

This is probaly the most asked question, so let's clarify this first of all.

No, the LP3 is **NOT a replacement** of the LP2 that does everything better. View them as **spoon vs fork** rather than **tea spoon vs table spoon**. They are simply *differet lasers for different purposes/materials*. Below is a table of supported materiels sourced from LP:

- Left: LP2 only
- Right: LP3 only
- Middle: supported by both

<img src="images/lp2_vs_lp3_materials.jpg" width="80%">

And I can confirm after testing that, although the LP3 seems so powerful that it can easily engrave all sorts of metals without needing a coating, it will not even scratch materials like paper, cardboard, wood, fabrics, ceramics, glasses, ... So think clearly what you wish to engrave before deciding which one to get.

It seems that getting both LP2 and LP3 will cover all the materials, and indeed many users do this. LP also thought about this, and made all LP2 add-ons, like the batch button, 3rd axis, including the stand, to be compatible with the LP3. The LP3 laser head as well as the upgraded stand will be sold separately to make it easier for loyal users to upgrade.

I just mentioned the upgraded stand that comes with the LP3. Let's have a look:

<img src="images/lp2_vs_lp3_01.jpg" width="48%"> <img src="images/lp2_vs_lp3_02.jpg" width="48%">
<img src="images/lp2_vs_lp3_03.jpg" width="48%"> <img src="images/lp2_vs_lp3_04.jpg" width="48%">
<img src="images/lp2_vs_lp3_05.jpg" width="48%"> <img src="images/lp2_vs_lp3_06.jpg" width="48%">
<img src="images/lp2_vs_lp3_09.jpg" width="48%"> <img src="images/lp2_vs_lp3_08.jpg" width="48%">
<img src="images/lp2_vs_lp3_07.jpg" width="48%">

It's not obvious in the photos, but the new stand is slightly taller, feels much sturdier and it has 2 additional guiding rods built-in to improve stability. I cross tested LP2, LP3 on the old and new stand. In short, although LP3 is much heavier than LP2, the old stand can support it just fine.

|  |Movement| LP2 (975g) | LP3 (1607g) |
| ------ | ------ | ------ | ------ |
| LP2 stand |Up| 200-220mA | 240-260mA |
|           |Down| 140-150mA | 140-160mA |
| LP3 stand |Up|165-175mA | 180-190mA |
|           |Down|140-150mA|140-150mA|


## Turn It On/Off

The LP3 can be turned off without unplugging the power cord by holding the "Play" button on its top for 3s.
To turn it back on, tap the same button once. If this did not work for you, make sure your LP2's firmware is up-to-date.


## What is A Field Lens?

In short, it is expensive and helps laser to focus on a flat engraving surface uniformly, despite it is projected from a sing static point.
Otherwise, the laser is only well focused in the centre area, and becomes out of focus as it moves away. The LP2 lacks such a field lens and therefore does not engrave as well where it is close to the edges and corners of the 100x100mm engraving area.

Below is a demo of *single line* engraving using Gcode. Note that the width of the line is uniform acoss the entire 90mm width.

<img src="images/lp3_single_line.jpg" width="80%">


## Finding the Optimal Engraving Distance

Although the manual suggests that the engraving surface should be *115mm* away from the button edge of the lens, my LP3 *test unit* was not calibrated to this. Yours may well be better calibrated, but it's still worth doing a few quick tests at slightly different heights/distances just to double check, and also get to know the tolerance of engraving distances/heights in case you wish to engrave something that's not perfectly flat.

### The Slope Test

Below is my "slope test" to find out the vertical engraving range using a sheet of SS. During preview, I used a marker to trace the engraving area, and used a ruler to measure the closest (107mm) and furthest (116mm) distancs. Finally, I just engraved a random image in Bin mode using the default setting for SS. In my case, the optimal engraving distance is 112mm ±1mm.

<img src="images/lp3_slope_test_01.jpg" width="60%"> <img src="images/lp3_slope_test_02.jpg" width="35%">
<img src="images/lp3_slope_test_03.jpg" width="48%">

Read below for next steps.

## Assist Red Lasers
### What they are
There are 3 assist red lasers in total. All of them are low power red lasers as visual aids. Just like red laser pointers.

One is internal. It only lights up when the LP3 is previewing or engraving. This one is aligned with the 1064nm invisible laser beam, purely to show where it is engraving.

<img src="images/lp3_assist_red_lasers2.jpg" width="50%">

Two of them can be seen at the buttom of the LP3. They will light up during preview, and can be manually turned on in app mode settings (`Red light stay`). They are to visually helping adjust the height of your engraver without using a ruler, provided the height they overlap at is the optimal height for engraving.

<img src="images/lp3_assist_red_lasers1.jpg" width="50%">

### Adjustment

If you found the optimal engraving height/distance for yours differs from what the red lasers indicate, the angle of the two red lasers can be adjusted using a suitable Allen key from the bottom of the LP3.

Steps:

1. Position your LP3 to the desired height.
2. Trn on the assist red lasers via app settings or just preview an engraving.
3. Turn the two screws **slowly and alternately** till the two red laser dots overlap on the engraving surface. Don't force it, or you might break it.

<img src="images/lp3_assist_red_lasers.jpg" width="50%">

