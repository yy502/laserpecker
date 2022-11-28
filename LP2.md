# Know Your LP2

## Turn It On/Off

moved to https://lp.systemd.one/?p=304

## Limitations by Design
moved to https://lp.systemd.one/?p=352


## Engraving Distance
moved to https://lp.systemd.one/?p=355


## Common Issues & Solutions

moved to https://lp.systemd.one/?p=359

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
9) (Optional) Reconnect to the factory calibration app. Wait about 5 seconds for the initial data transmission. Place a non-white paper under the engraver. Wear your laser goggles. Tap on this "G_code方圆雕刻" button to engrave a squares+circles image **on something not white** to verify the calibration.

<img src="images/ca04.jpg" width="600px">

<img src="images/ca05.jpg" width="600px">

## Factory Reset Firmware

In case of firmware update failure or issues with a new firmware, you can easily rollback to the factory firmware (v3.0.1) by:

1) Unplug power from your LP2
2) Plug in power to your LP2 and immediately press and hold the **two** circle buttons on the top of your LP2 until a red light comes up.
3) Release the buttons. The red light will go off and a blue light should start to flash on your LP2.

Reset completed.

## Update Firmware

Connect your LP2 to the LP mobile app, then go to app menu -> Version -> Version Update -> (update if a new version is found). Never ever update the firmware via the desktop version of LP apps.
