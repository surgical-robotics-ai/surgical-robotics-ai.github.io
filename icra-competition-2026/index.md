---
layout: default
---

# ICRA 2026 Competition: AI for Robotic Surgery

Surgical robotics is entering an exciting new era where the integration of artificial intelligence (AI) promises to improve the performance of human surgeons, and to address the growing shortage of surgeons and other medical personnel, thereby improving healthcare for all.

The most prevalent surgical robot in operating rooms today is the da Vinci Surgical System (Intuitive Surgical, Sunnyvale, CA), which has an installed base of more than 10,000 systems. The competition will use the da Vinci Research Kit (dVRK), an open-source research platform that re-purposes the mechanical hardware from retired clinical da Vinci Surgical Systems.

## Challenges

We will have two challenges, both using the peg transfer task.
In this task, the user picks up a peg from a post (with the non-dominant hand) and transfers it to another post, often with an intervening handoff between the left and right instruments without dropping the peg. This task (originating from the Fundamentals of Laparoscopic Surgery) is widely used in robotic surgery training to improve robotic manipulation skills, but is simple enough that anyone can learn it.

1. **Human teleoperated peg transfer:** the competitor uses an input device to teleoperate a real or simulated dVRK to transfer as many pegs as possible within the time limit.

2. **Autonomous peg transfer:** the competitor (or team) provides an AI algorithm to move a real or
simulated dVRK to transfer as many pegs as possible within the time limit. The algorithm must interface with the real or simulated dVRK using ROS2.

## Rules

- All competitors must sign a release form to allow their data to be collected and shared with the community.
- All pegs will start on posts on the left side of the workspace and must be transferred to posts on the right side.
Once all pegs are on the right side, the competitor must move them to the left side, and go back and forth until the
3-minute time limit expires.
- One point is awarded for each peg that is successfully placed on a post.
- There is no penalty for dropping a peg, though the time to recover is likely to reduce the final score.
- Direct human intervention, such as using hands to pick up dropped pegs, is not allowed. For example, if a peg is dropped and falls outside the robot workspace, the trial is stopped.
- Any incorrectly moved pegs (e.g., moving a peg from right to left before all pegs have been moved from left to right) will not be counted.
- If there is a hardware or software failure during a trial, the participant will be allowed to restart.
- There is no limit to the number of trials each competitor may attempt, but once a trial is completed,
the competitor must allow any other competitors to use the system.

## Assessment

- Performance will be assessed by the number of points (i.e., number of successfully placed pegs) within the
time limit.
- If multiple participants have the same number of points, the one who performed the task with the
least amount of PSM motion will be declared the winner.

## News

**November 16, 2025:** Website created

## Timeline

**Tues, June 2, 2026:** Human teleoperation competition (9 AM - 6 PM)

**Wed, June 3, 2026:** Human teleoperation and autonomous competition (9 AM - 6 PM)

**Thurs, June 4, 2026:** Autonomous competition (9 AM - 4 PM), Award ceremony, 4:45 PM (Hall C5)

## Awards

TBA

## Contact

To contact the organizers by email: [accelnet-robotics-challenge-admin@googlegroups.com](mailto:accelnet-robotics-challenge-admin@googlegroups.com)

## Acknowledgments

<p><img src="/images/NSF-logo.png" alt="NSF Logo" style="float:left; width:80px; height:80px; margin-right:25px">
Development of this Surgical Robotics Challenge is supported by the United States National Science Foundation (NSF)
via OISE-1927354 and OISE-1927275, <i>AccelNet: International Collaboration to Accelerate Research in Robotic Surgery</i>.</p>
