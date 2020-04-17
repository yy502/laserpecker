# # All About LaserPecker Automatic Stand

The automatic stand was released with the Pro model. It is compatible with L1 and can be purchased separately.

The stand folds up and fits into the carry case nicely. It does not have built-in battery. You will need one USB C cable to feed power to it; and it relays the power to the engraver via another short USB C cable. Both cables come along with the stand.

This stand can raise the engraver up to 29cm away from the base, meaning it can engrave objects up to 9cm thick, which covers most objects you want to engrave on. In case you want to engrave on very large objects, or engrave at certain angle, use the tripod that came with the engraver.

I have put a carbon-fibre sticker onto the base, and engraved a 100mm x 100mm grid over it to assist alignment of target objects. The grid is done via Gcode. I actually has 3 designs of the grids in Gcode files which can be found here: [yy502/inkscape-laserpecker/](https://github.com/yy502/inkscape-laserpecker/) in `misc` directory. 

<img src="images/es01.jpg" height="200px"><img src="images/es02.jpg" height="200px"><img src="images/es03.jpg" height="200px"><img src="images/es04.jpg" height="200px">

I was curious about its design, so I opened it up. It was easy. All the key components are in the rectangle shaped container. The plastic is stuck on with double sided tape. It does not require much effort to remove it.

Then, on the left, there are beeper, copper laser head for the 5-point guide (not a very useful feature in my opinion), and laser emitter + receiver for distance measurement.

In the middle, there's the fan for blowing smoke away for consistent engraving result.

On the right, connectors and the main processor.

<img src="images/es05.jpg" height="200px"><img src="images/es06.jpg" height="200px">


## Power Consumption

|State|Current (mA)|
| ------ | ------ |
| Off (Standby) | 30 |
| On | 415 |
| Moving up (with more resistance) |550-700|
| Hitting upper limit, before auto stopping|1120|
| Moving Down | 520-600|
