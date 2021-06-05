# Unofficial Guide to LaserPecker L1, L1 Pro & LP2

I am a happy owner of LaserPecker L1, L1 Pro and LP2. Here I document some of my usage and experience of using them. I may refer to L1 Pro as Pro for short in the rest of the articles.

Please note that my methods and settings are not necessarily the best. I have never used any laser engraver before, and these are the only ones I have for hobby use. I'll try to update my articles as I learn new tricks and test new materials.


# About LaserPecker

LaserPecker is brand of affordable and **portable** consumer level laser engravers. So far they have released their first generation laser engravers (L1 and L1 Pro) and their second generation laser engraver (LP2).

For more details, visit their official [English site](https://www.laserpecker.net/).


# Table of contents
## Generic Info
- [Online User Communities](#online-user-communities)
- [LaserPecker Fundamentals](#laserpecker-fundamentals)
  - [About the LaserPecker App](#about-the-laserpecker-app)
    - [Why Require Location Permision?](#why-require-location-permision)
    - [Offline Engraving](#offline-engraving)
    - [Registration & Satety PIN](#registration--satety-pin)
    - [Modes](#modes)
  - [Safety](#safety)
## LaserPecker 1
- [L1 & L1 Pro](/L1_index.md#l1--l1-pro)
  - [The Look](/L1_index.md#the-look)
  - [Key Specifications](/L1_index.md#key-specifications)
  - [Speed Comparison](/L1_index.md#speed-comparison)
- [Know Your Engraver](/L1_index.md#know-your-engraver)
  - [Valid Engraving Distance](/L1_index.md#valid-engraving-distance)
  - [Demos and Tips of L1](/L1.md)
  - [Demos and Tips of Pro](/Pro.md)
- [Automatic Stand](/Auto_Stand.md)
- [L1/Pro Modifications](/L1_index.md#l1pro-modifications)
## LaserPecker 2
- [LP2 Pre-Release Tests](LP2_pre_release_tests.md)







# Online User Communities

LaserPecker has large and friendly user communities on Facebook.

For 1st gen owners, please check out

* [LaserPecker VIP Group (official)](https://www.facebook.com/groups/laserpecker/)
* [LaserPecker User Group (unofficial)](https://www.facebook.com/groups/203376080793152/)

For 2nd gen owners, please check out

* [LaserPecker 2 VIP Group (official)](https://www.facebook.com/groups/374697760505822/)
* [LaserPecker 2 User Group (unofficial)](https://www.facebook.com/groups/lp2users/)


# LaserPecker Fundamentals

## About the LaserPecker App

_The App is updated frequently. My description here may be outdated._

Controlling the engraver is done via LaserPecker App in your smartphone over Bluetooth. The official desktop client is due to be released in March 2021.

Don't be put off by the low rating of the App in Play Store or App Store. It isn't perfect, but it's improving and updating frequently.

### Why Require Location Permision?
To Android users, the App requires **Location Permision** because Google made it that way, not that LaserPecker wants to know where you are. For your reference, read this [Android development documentation here](https://developer.android.com/guide/topics/connectivity/bluetooth#Permissions). To sumarise, it's because by allowing an App to perform a Bluetooth scan, it can potentially identify your location. To force-make users aware of this risk, any App that needs to scan for BLE (Bluetooth Low Energy) devices is forced to request Location Permission.

### Offline Engraving
Most people don't realise that, **once an engraving job is started, it is OK to quit the app or move your phone out of Bluetooth range.** You will lose the timer and progress info, and unable to carry on multi-pass engraving if you chose to engrave more than 1 pass, but you are free to do whatever you want while waiting for the engraving to finish.

Without the app, you can pause/resume the job by tapping on the **circle button** on the back of your engraver. Hold that button to cancel the job.

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




## Safety

Never ever look at the laser for long time (say, more than 10 seconds) when it's engraving, even with eye protections. It's OK to look at the laser in adjustment mode. It's low power.

I know it's hard to resist watching the ongoing engraving job, we have all done it ;-P If you must watch for whatever reason, turn on the camera app in your phone and watch over phone screen.



