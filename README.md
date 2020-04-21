# LaserPecker L1 & L1 Pro Review
I am a happy owner of both LaserPecker L1 and L1 Pro. Here I share some of my thoughts and uses of them. I may refer to L1 Pro as Pro for short in the rest of the article.


# LaserPecker
LaserPecker is brand of affordable and portable consumer level laser engravers. So far they have released their first generation laser engravers (L1 and L1 Pro). The company will release more models with more powerful capabilities in 2020 and the near future.

For more details, visit their official [English site](https://www.laserpecker.net/) or [Chinese site](http://www.laserpecker.cn/).


# L1 vs L1 Pro

## The Look
L1 and Pro are of the same size & design, with minor difference as shown below. Therefore both will fit onto the automatic stand. 

![](images/L1_vs_Pro.jpg)


## Key Specifications

|  | L1 | L1 Pro |
| ------ | ------ | ------ |
| Laser | 450nm Blue, 1600mW | 405nm Blue-Violet, 500mW (equivalent to 1500mW Blue laser) |
| Pixel Size | 0.3mm (or smaller\*)| 0.15mm |
| Engrave Range|100mm x 100mm (or larger\**)| 100mm x 100mm (or larger\*\*\*)|


\* Can be improved with an easy modification, but engraving range will reduce as a trade-off. Read on.

\*\* Up to 200mm x 140mm with Gcode. Read my L1 review.

\*\*\* Up to 106mm x 106mm with Gcode, but the improvement is so small that it's not worth the trouble.


# L1 Review (being updated...)

[Click here](L1_EN.md)


# L1 Pro Review (being updated...)

[Click here](Pro_EN.md)


# Automatic Stand

[Click Here](Auto_Stand_EN.md)


# Speed Comparison

Due to Pro's increased precision, it takes up to **four** times long to engrave the same amount of pixels. I have tested every depth setting available in the App, and have produced the graph below. It shows how much time a Pro takes compared to an L1.

<img src="images/pro_to_L1.png">


# LaserPecker App

Controlling the engraver is done via LaserPecker App in your smartphone over Bluetooth. I do wish there's a desktop (Linux particularly) client or API available, as I'm a big fan of automation via scripting.

Don't be put off by the low rating of the App in Play Store or App Store. It isn't perfect, but it's improving and updating frequently.

There are 5 modes for image processing:
1) **Pencil**: Converts image to pencil sketch style via edge detection.
2) **G-code**: Converts image to vector paths via edge detection, mainly for cutting with (100,100) setting.
3) **Bin**: Binary, i.e. black & white mode. It converts your image to black and white for engraving.  
4) **Gray**: Converts your image to gray scale. However, the engraving results may not be as good as you expect. Material is very important. MDF boards are very good for this. Try it out for yourself. Be warned that engraving gray scale image is **very** slow, as every pixel is engraved.
5) **Seal**: Inverts your desired image/pattern for making stamps.

Known bug (Android): if the App has connected to the engraver, and you hit Back button a few times to get back to the initial page before choosing an engraver to connect to; and then try to search for the engraver, the App won't find any. You will need to force kill the App, and the relaunch it to start over. A little annoying, but it's not the end of the world.

