# LaserPecker L1 & L1 Pro Review
I am a happy owner of both LaserPecker L1 and L1 Pro. Here I share some of my thoughts and uses of them. I may refer to L1 Pro as Pro for short in the rest of the article.


# LaserPecker
LaserPecker is brand of affordable and **portable** consumer level laser engravers. So far they have released their first generation laser engravers (L1 and L1 Pro). Their second generation portable engraver has been recently released via [KickStarter](https://www.kickstarter.com/projects/laserpecker-pro/laserpecker-2-the-best-handheld-laser-engraverandcutter).

For more details, visit their official [English site](https://www.laserpecker.net/) or [Chinese site](http://www.laserpecker.cn/).


# L1 vs L1 Pro

## The Look
L1 and Pro are of the same size & design, with minor difference as shown below. Therefore both will fit onto the automatic stand. 

![](images/L1_vs_Pro.jpg)


## Key Specifications

|  | L1 | L1 Pro |
| ------ | ------ | ------ |
| Laser | 450nm Blue, 1600mW | 405nm Blue-Violet, 500mW (equivalent to 1500mW) |
| Pixel Size | 0.3mm (or smaller\*) | 0.15mm |
| Engrave Range|100mm x 100mm | 100mm x 100mm |

\* Can be improved with an easy modification, but engraving range will reduce as a trade-off. Read on.


# [L1 Review](L1_EN.md)

# [L1 Pro Review](Pro_EN.md)

# [Automatic Stand](Auto_Stand_EN.md)
* [Noisy Fan & Replacement](Auto_Stand_EN.md#noisy-fan--replacement)

# Modifications
* [Kick-ass mod to improve L1 accuracy and power](/L1_EN.md#kick-ass-modification-cheap--cheerful)
* [Laser guide add-on to assist alignment for both L1 and L1 Pro](/modifications.md#laser-guide-add-on-to-assist-alignment-for-both-l1-and-l1-pro)
* [Flip adaptor for auto-stand](/modifications.md#flip-adaptor-for-auto-stand)
* [4-way placement extension for auto-stand](/modifications.md#4-way-placement-extension-for-auto-stand)
* [3-way compact adaptor for auto-stand](/modifications.md#3-way-compact-adaptor-for-auto-stand)


# What LaserPecker Don't Tell You...

## About the LaserPecker App

_The App is updated frequently. My description here may be outdated._

Controlling the engraver is done via LaserPecker App in your smartphone over Bluetooth. The official desktop client is due to be released in March 2021.

Don't be put off by the low rating of the App in Play Store or App Store. It isn't perfect, but it's improving and updating frequently.

### Why Require Location Permision?
To Android users, the App requires **Location Permision** because Google made it that way, not that LaserPecker wants to know where you are. For your reference, read this [Android development documentation here](https://developer.android.com/guide/topics/connectivity/bluetooth#Permissions). To sumarise, it's because by allowing an App to perform a Bluetooth scan, it can potentially identify your location. To force-make users aware of this risk, any App that needs to scan for BLE (Bluetooth Low Energy) devices is forced to request Location Permission.

Most people don't realise that, **once an engraving job is started, it is OK to quit the app or move your phone out of Bluetooth range.** You will lose the timer and progress info, but you are free to do whatever you want while waiting for the engraving to finish.

Without the app, you can pause/resume the job by tapping on the circle button on the back of your engraver. Hold that button to cancel the job.

### Registration & Satety PIN
The initial registration process works as below:
1. Enter your email address and get a verification code sent to it. At the same time, the code is sent to the app in the background to be verified against.
2. Wait for the verification email. Check your Spam/Junk folder. **Do not repeatedly click on "Send Code" button in the app.** You will end up getting multiple verification emails, but only the last one is valid. So it does not descrease your wait time but to make it worse.
3. Once you get the verification code and set your safety PIN, the PIN is **stored in the engraver**.
4. When you use your engraver with a fresh install of the LP app, in your current device or a different device, you only need to verify the safety PIN at the bottom of the registration page. There's no need to reregister.

If you transfer your device to a different user, he/she can go through the registration process like you did and overwrite the safety PIN.


### Modes
There are **5 modes** for image processing:
1) **Pencil**: Converts image to pencil sketch style via edge detection.
2) **G-code**: Converts image to vector paths via edge detection, mainly for cutting with (100,100) setting. You can add different levels of line-fill in the dark area of the original image byt sliding the slider dot to the right. On the very right end you will get 100% fill by lines. It is not necessarily faster than directly using Bin mode, depending on the complexity of your image. Try it out to see what works better for you. Personally, I find 50% fill works pretty well for wood. **Note that Gcode mode is secretly about 2x powerful than other modes suing the same setting.** For example, I found that Gcode (70,30) produces about the same result as Bin (100,70). Potentially you can lower the depth setting to speed up your job.
3) **Bin**: Binary, i.e. black & white mode. It converts your image to black and white for engraving.  
4) **Gray**: Converts your image to grayscale. Your iamge may look nice in the App, but the engraving result is most likely as good as you expect. Material is very *very* **very** important. MDF boards and thick brown paper are pretty good for this. Try it out for yourself. Be warned that engraving gray scale image is **very** slow, as every pixel is engraved with varying power/depth settings. Don't be disappointed if your result misses half of the details. Think of it this way, all the gray pixels in your image are coverted to different powers of laser pulses, let's say from level 1 to level 10, to achieve 10 levels of burn, in theory. However, in reality your matierial does not get burnt up to power level 5; and it gets burnt equally dark from level 9 to 10. So all the pixels that are meant to be burnt with power level 1 to 5 won't show. And all the pixels burnt with power 9 and 10 become indistinguishable. As a result, the 10-level grayscale image becomes 4-level only (level 6, 7, 8, 9+10). This is a common challenge in laser engraving. And the solutionm is to dither your image (i.e. to use different densities of black & white pixes to emulate grayscale) and use Bin mode to engrave it. Here is a free online tool for this http://imag-r.com/.
5) **Seal**: Inverts your desired image/pattern for making stamps. To be used with photosensitive stamps.

The Creation mode is being actively developed. It now supports custom fonts. Note that if you set your texts to hollow style, they will be engraved with Gcode mode. i.e. the laser will trace each character's outline rather than scanning through line by line.


## L1 vs Pro Speed Comparison

Due to Pro's increased precision, it takes up to **four** times long to engrave the same amount of pixels. I have tested every depth setting available in the App, and have produced the graph below. It shows how much time a Pro takes compared to an L1.

Some quick numbers to note:

* at up to 75% depth, Pro performs very similarly to L1.
* at 80-85% depth, Pro takes about 1.5 times long compared to L1.
* at 90% depth, Pro takes about 2 times long compared to L1.
* at 95% depth, Pro takes about 2.5 times long compared to L1.
* at 100% depth, Pro takes about 4 times long compared to L1.


<img src="images/pro_to_L1.png">


# Safety

Never ever look at the laser for long time (say, more than 10 seconds) when it's engraving, even with eye protections. It's OK to look at the laser in adjustment mode. It's low power.

I know it's hard to resist watching the ongoing engraving job, we have all done it ;-P If you must watch for whatever reason, turn on the camera app in your phone and watch over phone screen.
