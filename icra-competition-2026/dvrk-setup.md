---
layout: default
---

## Physical dVRK Setup

There will be two PSMs from the first-generation [da Vinci Research Kit (dVRK)](https://dvrk.readthedocs.io/main/), mounted on a fixed frame. A large needle driver (LND) will be installed in each PSM. We will use a fixed stereo camera (OAK-D-SR) to emulate a modern clinical endoscope (which has better image quality than the standard dVRK endoscope). A pegboard with pegs will be positioned between the two PSMs.

The physical setup will use two computers:  (1) dVRK Control PC, connected to the dVRK controllers via FireWire, and (2) Video PC, connected to the stereo camera and Quest 3 (for human teleoperation trials). The two computers will be connected together via a local network.

Following is a photo of the Physical dVRK setup:  TBD

## Human Teleoperation Peg Transfer Challenge

No preparation is necessary -- please come to the competition area and give it a try!

You will use a Quest 3 HMD, with hand controllers, as the interface to control the physical PSMs.

## Autonomous Peg Transfer Challenge

Competitors for the Autonomous Peg Transfer Challenge should consider one or more of the following options:

### Option 1: Run your algorithm on your own computer

Your computer should be running ROS2 Jazzy(?) and can interface to the Video PC via a local area connection.

### Option 2: Run your algorithm on the Video PC

We will create a separate login account for your team, using the account name requested on the registration form.

Following are the specifications for the Video PC: TBD

In addition to ROS2, the following packages will be installed: TBD

## Video Specifications

The physical setup uses an OAK-D-SR stereo camera instead of an endoscope. Specifications are available [here](https://shop.luxonis.com/products/oak-d-sr). Key specifications include the following:

* Stereo baseline:  20 mm
* FOV: 80 deg (H), 55 deg (V)
* Resolution:  1280 x 800

Interface to the stereo video stream is provided by gstreamer. Details TBD.

Although this camera can provide depth estimates using its onboard processing, this feature will not be available for the competition to preserve some similarity to a clinical endoscope. However, competitors are allowed to implement their own depth estimation using the stereo images.
