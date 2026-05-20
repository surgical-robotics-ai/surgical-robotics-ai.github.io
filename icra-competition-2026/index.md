---
layout: default
---

# ICRA 2026 Competition: AI for Robotic Surgery

Surgical robotics is entering an exciting new era where the integration of artificial intelligence (AI) promises to improve the performance of human surgeons, and to address the growing shortage of surgeons and other medical personnel, thereby improving healthcare for all.

The most prevalent surgical robot in operating rooms today is the da Vinci Surgical System (Intuitive Surgical, Sunnyvale, CA), which has an installed base of more than 10,000 systems. The competition will use the da Vinci Research Kit (dVRK), an open-source research platform that re-purposes the mechanical hardware from retired clinical da Vinci Surgical Systems.

## Challenges

We will have two challenges, both using the peg transfer task.
In this task, the user picks up a peg from a post (with the non-dominant hand) and transfers it to another post, often with an intervening handoff between the left and right instruments without dropping the peg. This task (originating from the Fundamentals of Laparoscopic Surgery) is widely used in robotic surgery training to improve robotic manipulation skills, but is simple enough that anyone can learn it.

We have increased the task difficulty by introducing a barrier (wall) in between the left and right sides of the pegboard. This barrier, and workspace constraints, make it impossible to perform the task without a handoff between the two instruments.

1. **Human teleoperated peg transfer:** the competitor uses an input device (Meta Quest 3) to teleoperate a real or simulated dVRK to transfer as many pegs as possible within the time limit.

2. **Autonomous peg transfer:** the competitor (or team) provides an AI algorithm to move a real or simulated dVRK to transfer as many pegs as possible within the time limit. The algorithm must interface with the real or simulated dVRK using ROS2.

## Environments

We will have both simulated and physical setups on the competition floor. The intent is for the two setups to be as similar as possible.
Both setups will use Ubuntu 24.04 and ROS 2.

The Patient Side Manipulators (PSMs) and camera will not be moved and we will provide all transformations between them, including stereo camera calibration (intrinsic and extrinsic parameters). The peg board location will not be provided and may move during the competition.

Each setup will include a Meta Quest 3 connected to the computer via an Ethernet/USB-C adapter. This tethered configuration was chosen to avoid potential issues with WiFi connections in the exhibit hall, and to allow continuous charging of the devices.

Following are details about the three different environments:

* [AMBF Simulation Setup](./ambf-setup.html)
* Isaac Sim Setup
* [Physical dVRK Setup](./dvrk-setup.html)

The ROS2 API for all three setups is the same, and is documented here:  TBD

## Competition Rules and Assessment

* See [this page](./rules.html)

## News

**November 16, 2025:** Website created

**May 11, 2026:** Details added

**May 19, 2026:** More details added

## Timeline

**Tues, June 2, 2026:** Human teleoperation competition (9 AM - 6 PM)

**Wed, June 3, 2026:** Human teleoperation and autonomous competition (9 AM - 6 PM)

**Thurs, June 4, 2026:** Autonomous competition (9 AM - 4 PM), Award ceremony, 4:45 PM (Hall C5)

## Registration (ICRA and Competition)

All competitors must be registered for ICRA. In addition, teams interested in the Autonomous competition register for the challenge, using the link TBA. Registration will give access to the calendar for scheduling time to test your algorithm on the physical or simulated system.

The Human Teleoperation challenge is only open to individuals (not teams) and there is no registration for the challenge--just show up and give it your best!

If you would like to participate in any of the challenges, but are not registered for ICRA, a 'competition only' registration rate may be available (please contact us to check).

## Awards

The top performers in the following categories will receive prizes (in Euros) and a certificate at the awards ceremony:

| Competition                    | 1st place  | 2nd place  | 3rd place  | Total |
|--------------------------------|------------|------------|------------|-------|
| Human Teleoperation, AMBF Sim  |     125    |     50     |     25     |  200  |
| Human Teleoperation, Isaac Sim |     125    |     50     |     25     |  200  |
| Human Teleoperation, Real      |     250    |    100     |     50     |  400  |
| Autonomous AI, AMBF Sim        |     300    |    150     |     50     |  500  |
| Autonomous AI, Isaac Sim       |     300    |    150     |     50     |  500  |
| Autonomous AI, Real            |     600    |    300     |    100     | 1000  |
| TOTAL                          |            |            |            | 2800  |

The prizes will be given as Virtual Visa gift cards, a few weeks after the conclusion of the competition.

**Note:** If the second simulation environment uses AMBF instead of Isaac Sim, the Sim categories will be combined.

## Contact

To contact the organizers by email: [accelnet-robotics-challenge-admin@googlegroups.com](mailto:accelnet-robotics-challenge-admin@googlegroups.com)

## Acknowledgments

<p><img src="/images/NSF-logo.png" alt="NSF Logo" style="float:left; width:80px; height:80px; margin-right:25px">
Development of this Surgical Robotics Challenge is supported by the United States National Science Foundation (NSF)
via OISE-1927354 and OISE-1927275, <i>AccelNet: International Collaboration to Accelerate Research in Robotic Surgery</i>.</p>
