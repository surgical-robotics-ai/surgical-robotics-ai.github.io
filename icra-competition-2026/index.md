---
layout: default
---

# ICRA 2026 Competition: AI for Robotic Surgery

Surgical robotics is entering an exciting new era where the integration of artificial intelligence (AI) promises to improve the performance of human surgeons, and to address the growing shortage of surgeons and other medical personnel, thereby improving healthcare for all.

The most prevalent surgical robot in operating rooms today is the da Vinci Surgical System (Intuitive Surgical, Sunnyvale, CA), which has an installed base of more than 10,000 systems. The competition will use the da Vinci Research Kit (dVRK), an open-source research platform that re-purposes the mechanical hardware from retired clinical da Vinci Surgical Systems.

## Challenges

We will have two challenges, both using the peg transfer task.
In this task, the user picks up a peg from a post (with the non-dominant hand) and transfers it to another post, often with an intervening handoff between the left and right instruments without dropping the peg. This task (originating from the Fundamentals of Laparoscopic Surgery) is widely used in robotic surgery training to improve robotic manipulation skills, but is simple enough that anyone can learn it.

1. **Human teleoperated peg transfer:** the competitor uses an input device (Meta Quest 3) to teleoperate a real or simulated dVRK to transfer as many pegs as possible within the time limit.

2. **Autonomous peg transfer:** the competitor (or team) provides an AI algorithm to move a real or
simulated dVRK to transfer as many pegs as possible within the time limit. The algorithm must interface with the real or simulated dVRK using ROS2.

## Environments

We will have both simulated and physical setups on the competition floor. The intent is for the two setups to be as similar as possible.
Both setups will use Ubuntu 24.04 and ROS 2.

The Patient Side Manipulators (PSMs) and camera will not be moved and we will provide all transformations between them, including stereo camera calibration (intrinsic and extrinsic parameters). The peg board location will not be provided and may move during the competition.

Each setup will include a Meta Quest 3 connected to the computer via an Ethernet/USB-C adapter. This tethered configuration was chosen to avoid potential issues with WiFi connections in the exhibit hall, and to allow continuous charging of the devices.


### Simulation Setup

There will be two computers running simulated environments: one based on the [Asynchronous Multi-Body Framework (AMBF)](https://github.com/WPI-AIM/ambf) and the other is expected to use Isaac Sim (with AMBF as a backup). All simulation assets will be available through the
[Surgical Robotics Challenge Assets](https://github.com/surgical-robotics-ai/surgical_robotics_challenge).

The simulation environment will be similar to the one below. There will be two da Vinci large needle drivers and a pegboard with three pegs. Each peg will be a different color. There will be obstacles on the pegboard.

<img src="./AMBF-screenshot.jpg" alt="AMBF Simulation" style="width:600px">

### Real Setup

There will be two PSMs from the first-generation [da Vinci Research Kit (dVRK)](https://dvrk.readthedocs.io/main/), mounted on a fixed frame. A large needle driver (LND) will be installed in each PSM. We will use a fixed stereo camera (OAK-D-SR) to emulate a modern clinical endoscope (which has better image quality than the standard dVRK endoscope). A pegboard with pegs will be positioned between the two PSMs.

The real setup will use two computers:  one connected to the dVRK controllers via FireWire, and one connected to the stereo camera and the Quest 3 (for human teleoperation trials). The two computers will be connected together via a local network.

## Rules

- All competitors must sign a release form to allow their data to be collected and shared with the community.
- All 3 pegs will start on posts on the left side of the workspace and must be transferred to posts on the right side, with a handoff from one instrument to the other.
Once all pegs are on the right side, the competitor must move them to the left side, and go back and forth until the
3-minute time limit expires.
- One point is awarded for each peg that is successfully placed on a post.
- There is no penalty for dropping a peg, though the time to recover is likely to reduce the final score.
- Direct human intervention, such as using hands to pick up dropped pegs, is not allowed. For example, if a peg is dropped and falls outside the robot workspace, the trial is stopped.
- Any incorrectly moved pegs (e.g., moving a peg from right to left before all pegs have been moved from left to right) will not be counted.
- If there is a hardware or software failure during a trial, the participant will be allowed to restart.
- There is no limit to the number of trials each competitor may attempt, but once a trial is completed,
the competitor must allow any other competitors to use the system.
- Competitors may participate in any of the challenges, but can win at most one award in each challenge. For example, if a competitor has the top three scores in the "Human Teleoperation, Real" challenge, they will be awarded first place, but will not receive the second or third place awards.

## Assessment

- Performance will be assessed by the number of points (i.e., number of successfully placed pegs) within the
time limit.
- If multiple participants have the same number of points, the one who performed the task with the
least amount of PSM motion will be declared the winner.

## News

**November 16, 2025:** Website created

**May 11, 2026:** Details added

## Timeline

**Tues, June 2, 2026:** Human teleoperation competition (9 AM - 6 PM)

**Wed, June 3, 2026:** Human teleoperation and autonomous competition (9 AM - 6 PM)

**Thurs, June 4, 2026:** Autonomous competition (9 AM - 4 PM), Award ceremony, 4:45 PM (Hall C5)

## Registration (ICRA and Competition)

All competitors must be registered for ICRA. In addition, teams interested in the Autonomous competition register for the challenge, using the link TBA. Registration will give access to the calendar for scheduling practice time with the system.

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
