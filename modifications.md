# Table of contents

- [Mods for L1/L1 Pro](#mods-for-l1l1-pro)
  - [Laser Guide Add-On to Assist Alignment](#laser-guide-add-on-to-assist-alignment)
  - [Flip Adaptor for Auto-Stand](#flip-adaptor-for-auto-stand)
  - [4-Way Placement Extension for Auto-Stand](#4-way-placement-extension-for-auto-stand)
  - [3-Way Compact Adaptor for Auto-Stand](#3-way-compact-adaptor-for-auto-stand)
- [Mods for LP2](#mods-for-lp2)
  - [Engraving Distance Probe](#engraving-distance-probe)
  - [Double Distance Probe](#double-distance-probe)
  - [Vent Deflector](#vent-deflector)
  - [3rd Axis Supports](#3rd-axis-supports)
  - [Power Bank Holder](#power-bank-holder)

# Mods for L1/L1 Pro

moved to https://lp.systemd.one/?p=384

## Flip Adaptor for Auto-Stand

moved to https://lp.systemd.one/?p=408


## 4-Way Placement Extension for Auto-Stand
moved to https://lp.systemd.one/?p=410


## 3-Way Compact Adaptor for Auto-Stand

moved to https://lp.systemd.one/?p=417

# Mods for LP2

moved to https://lp.systemd.one/?p=419

## Double Distance Probe

Compared to the single prove, this one offers: (1) hand-free measurement; (2) ensures the engraver is parallel to a large surface/object when tilted (see the last image in the video demo). Mind that this one is a bit difficult to print and clean up.

### Printing Instructions

* [LP2 110mm double probe (stl file)](/misc/LP2_110mm_double_probe.stl)
    * enable support
    * use 15%+ infill and **0.1mm** layer height
    * depending on your printer and filament, you may need to reduce flow a little bit.
    * After printing, carefully separate the `/` design with a shape knife so that the end of the probes can retract when pressed.
    * Carefully observe the bottom of the hinge in an STL viewer or slicer, then use a sharp knife to separate the designed gaps in the first layer that may be stuck together due to elephant foot effect or use of brim. I highly recommend you do a [test print of the hinge only](/misc/LP2_110mm_double_probe_test.stl) to see if your print settings need adjusting at all, before spending 3-4 hours printing the complete design. 

### Usage

Slide the printed part onto the bottom of the LP2, and lower the engraver till the tip(s) of the probe(s) touch the engraving surface without retraction.

The probes can be flipped up when not in use. They are designed to stay at the horizontal position without dropping.

Click to watch demo:

[![](https://img.youtube.com/vi/BrNvzurz91k/0.jpg)](https://www.youtube.com/watch?v=BrNvzurz91k)

<img src="images/mod56.png" height="220px"> <img src="images/mod57.png" height="220px">

## Vent Deflector

This is needed only when you engrave very light material, such as embossing powder, or cutting thin paper, so that the airflow from the vent holes does not blow yuor material away during engraving.

### Part
* 3D printed [vent deflector (stl file)](/misc/LP2_vent_deflector.stl)
    * no support needed
    * 15%+ infill, 0.1-0.2mm layer height

### Usage
You may keep it on the engraver and slide it to the desired position as needed.

<img src="images/mod47.jpg" height="280px"> <img src="images/mod48.jpg" height="280px">


## 3rd Axis Supports

This is a 3-piece set. They help you place a cone shaped object on the 3rd axis addon for engaving. If you place a cone on the rollers directly without this support, you will have 2 issues:

1) the top side to be engraved on is not horizontal, so it's difficult to alighn it with the engraver.
2) as the rollers roll the cone shaped object by contact, the big end and small end would be moving at different angular velocity, and therefore the whole object may skid or come off the rollers. It's a simple maths/geometry issue, not that the 3rd is faulty or anything.

As a solution, I designed this support to raise the small end of the object and to allow the small end to freely rotate at the same angular velocity as the big end moved by the rollers, solving exactly the 2 issues described above.

The end stopper (the big clip, AKA part C) stops the object from moving sideways by gravity. So all 3 parts are required.

In addition, since the final version of the 3rd axis rollers are metal instead of rubber, there's a big chance that the object may skid sicne the contact area is very small and on hard metal surface. A simple solution is to put a rubber band on the end of the cone to increase friction.

### Parts
* 3D printed [part A](/misc/LP2_3rd_Axis_support_A.stl), [part B](/misc/LP2_3rd_Axis_support_B.stl) and [part C](/misc/LP2_3rd_Axis_support_C.stl)
   * need support
   * 15%+ infill, 0.1-0.2mm layer height

### Usage
* Adjust height of the end support with a stable flat object.
* Adjust spacing according to your object.
* Centre-align the end support.
* Place your object on the rollers, make sure the top of it is horizontal.
* Finally place the end stopper (the big clip) to stop it from moving during rolling.

Here is [an illustration of positioning the support](https://www.facebook.com/groups/374697760505822/permalink/466559177986346/) and [a demo of how to use it to engrave on a cone](https://www.facebook.com/groups/374697760505822/permalink/472151160760481/).

<img src="images/mod50.jpg" height="280px"> <img src="images/mod51.jpg" height="280px">

<img src="images/mod49.jpg" height="280px">

## Power Bank Holder

This holder snaps and locks onto the LP2 by itself, and keeps the power bank attached to the main unit for easy handheld engravings.

### Part
* 3D printed [LP2 Power Bank Holder (stl file)](/misc/LP2_power_bank_holder.stl)
  * Print at 135 degrees (longest side face down) to reduce the need of support.
  * 15% infill, 0.2mm layer height

<img src="images/mod52.png" height="300px"> <img src="images/mod53.png" height="300px">


### Usage
Click the image below to watch a video demo.

[![](https://img.youtube.com/vi/Tx-IJ6oXi0o/1.jpg)](https://www.youtube.com/watch?v=Tx-IJ6oXi0o)

<img src="images/mod54.jpg" height="300px"> <img src="images/mod55.jpg" height="300px">
