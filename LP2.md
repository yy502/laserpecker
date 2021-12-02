# Know Your LP2

## Turn It On/Off

As of firmware v3.0.7, the LP2 can be turned off without unplugging the power cord by press and hold the "Play" button on its top for 3 seconds. To turn it back on, short tap the same button.

## Limitations by Design
Since the laser source is static on the engraver, it will project to a very small central area at approximately 90 degrees with the best focus spot (0.05mm).
As the laser moves to the edges and corners of the max engraving area (100mm x 100mm), the projection angle reduces and the laser spot become an oval, which
means the focused power will be weaker and the engraving quality degrades. See [Test #29: Faded Corners at Max Size](https://www.facebook.com/groups/374697760505822/permalink/444594843516113/)
and [Test #44: Dealing with Faded Corners](https://www.facebook.com/groups/374697760505822/permalink/452307826078148/).

Another side effect is that when cutting large thick material, the bottom layer will be larger than the top layer. I've done some maths below to show what the
differences are at the edge and corner with 3mm and 5mm thick material. 

<img src="images/LP2_laser_projection.png" height="900px">


## Engraving Distance

LP2's optimal engraving distance is `110±1mm` (i.e. 109-111mm). Too close or too far will result in uneven results when you engrave a large-ish area, say over 65mm x 65mm.
If you are unsure about it, test on some scrap material after setting the engraving distance.

### Cutting Thick Material
If you cut sheet material that is more than 3mm thick, it is recommended to set your engraving distance to `110mm - material_thickness/2`,
so that the perfect 110mm focus point falls in the middle of the material to be cut. In this way, the laser will be out of optimal focus by half
material thickness at most. Otherwise, it will be out of focus by 100% material thickness as it cuts through to the bottom side of the material.
See demo of cutting 5.5mm wood in [Test #63: Mixed Materials](https://www.facebook.com/groups/374697760505822/permalink/494716925170571/).

<img src="images/LP2_engraving_distance_flat.png" height="800px">

### Curved Surface
Because the optimal engraving depth is only 2mm (`110±1mm`), to minimise the amount the laser becomes out of focus when engraving on a curved
surface which has varying distance to the engraver, you should estimate the depth of the engraving area and offset the engraving distance by half of it.

Again, you may want to do some tests to check the engraving quality at slightly different distances before doing the "real job".

<img src="images/LP2_engraving_distance_curve.png" height="800px">



## Common Issues & Solutions

### My engraver won't connect to the app.

If your engraver has a flshing blue light, it's standing by for connection. If you use an Android phone, enable GPS so the app can search nearby Bluetooth devices.

If your engraver has a flashing green or yellow light after powering on, it's faulty. Contact the seller to arrange a replacement.

### OMG! My stand moves up and down randomly by itself!

Don't worry. It's becasue the AC socket you used was not properly earthed/grounded, so there were some interferences that caused this.

Just use a different AC socket (on the wall, not on the same extenison board).

## Factory Calibration

### WARNING
**YOU COULD BRICK YOUR LP2 AND VOID YOUR WARRANTY!!**

**YOU COULD BRICK YOUR LP2 AND VOID YOUR WARRANTY!!**

**YOU COULD BRICK YOUR LP2 AND VOID YOUR WARRANTY!!**

* I am sharing this guide based on my own experience, and I am not responsible for potential damage to your engraver.
* **ONLY** do this when your engraving is visibly distorted and you are told to do so by LaserPecker tech support. This should be a one-off process and you should not do this often just because you can.
* Do **NOT** try any other button in the app!

**YOU COULD BRICK YOUR LP2 AND VOID YOUR WARRANTY!!**

**YOU COULD BRICK YOUR LP2 AND VOID YOUR WARRANTY!!**

**YOU COULD BRICK YOUR LP2 AND VOID YOUR WARRANTY!!**

### Requirements

1) Print this [calibration reference sheet](/misc/LP2_calibration_reference.pdf) and an A4 paper and cut it along the outline. **Ensure the cutout perfectly matches the base of the stand. Otherwise, the scaling is wrong and it will mess up the calibration if you use it.**

<img src="images/ca01.jpg" height="400px"> <img src="images/ca02.jpg" height="400px">

2) Use an Android phone, install LP2 factory calibration app [(apk file)](/misc/LP2_factory_calibration.apk). After installation, it looks like this:

<img src="images/ca03.jpg" height="200px">

### Procedures

Click to watch a video demo of the whole process.

[![](https://img.youtube.com/vi/Xw3VQ97L7yE/3.jpg)](https://www.youtube.com/watch?v=Xw3VQ97L7yE)


1) Place the calibration reference sheet onto the base of the stand. It should match the size of the base plate perfectly, otherwise your print is in a wrong size.
2) Mount your LP2 onto the electric stand, lower it to the lowest position.
3) Launch the factory calibration app. Select L2 on the top and then tap on your LP2 when it is discovered.
4) Wait a few seconds until the red texts in the middle of the screen become "数据处理完成" (it means "data processed").
5) Tap on any of the direction button to light up the laser and start calibration.
6) Use the direction buttons to move the laser spot to its closest reference point, then tap on the gray Confirm button. Laser spot then moves to the next calibration point.
7) Repeat step 6 until the laser spot returns to the centre and turns off. Now wait for a long beep and the laser lights up again in the centre. It will finally continuously trace the 100x100mm square. This is the end of calibration.
8) Power off your LP2 and then power it back up.
9) (Optional) Reconnect to the factory calibration app. Wait about 5 seconds for the initial data transmission. Place a non-white paper under the engraver. Wear your laser goggles. Tap on this "G_code方圆雕刻" button to engrave a squares+circles image to verify the calibration.

<img src="images/ca04.jpg" width="600px">

<img src="images/ca05.jpg" width="600px">

## Factory Reset Firmware

In case of firmware update failure or issues with a new firmware, you can easily rollback to the factory firmware (v3.0.1) by:

1) Unplug power from your LP2
2) Plug in power to your LP2 and immediately press and hold the **two** circle buttons on the top of your LP2 until a red light comes up.
3) Release the buttons. The red light will go off and a blue light should start to flash on your LP2.

Reset completed.

## Update Firmware

Connect your LP2 to the LP mobile app, then go to app menu -> Version -> Version Update -> (update if a new version is found).
