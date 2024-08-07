---
layout: default
---

# 2023-2024 AccelNet Surgical Robotics Challenge

This is a relaunch and update of the
[2021-2022 AccelNet Surgical Robotics Challenge](../surgical-robotics-challenge-2021/challenge-2021.md).
As with the prior challenge, the goal is to further advance research in the
automation of surgical subtasks during robot-assisted surgery.
The primary changes are:
  * The challenge consists of an online phase (in simulation) followed by an in-person phase (with physical hardware)
  * The simulation environment uses SI units to better match the physical environment
  * The simulation environment uses models of real phantoms
  * The simulation environment uses a more realistic model of the surgical instrument
  * The accuracy of the simulated robots is consistent with that of the physical robots
  * The stereo endoscope video in the physical setup is consistent with that of the simulated environment (i.e., will be higher quality)

In this challenge, we provide the specifications for multiple physical platforms that each consist of two
seven degrees-of-freedom (DOF) instrument arms based on the da Vinci Surgical System
large needle driver, a controllable stereo camera,
a suturing phantom, and a needle with suture.
Note that the stereo camera has higher quality than the stereo endoscope provided with
the first-generation da Vinci surgical system.
We also provide a simulation environment for each specified physical platform.
The goal is to conduct the first part of the challenge in simulation, followed by a sim-to-real transfer
on the physical platforms. The following video provides a "teaser" of the updated simulation environment.

<video width="800" height="540" autoplay muted loop>
  <source type="video/mp4" src="/surgical-robotics-challenge-2023/Suturing-AMBF.mp4">
Your browser does not support the video tag.
</video>

## News

**May 28, 2024:** The effort to improve the simulator to better match the physical system has taken longer than expected, and we expect to update the [surgical_robotics_challenge repository](https://github.com/surgical-robotics-ai/surgical_robotics_challenge) within the next week. As a result, we will be revising the timeline.

**July 12, 2024:** Released v2.0.0 of the [surgical robotics challenge](https://github.com/surgical-robotics-ai/surgical_robotics_challenge). See the [Change Log](https://github.com/surgical-robotics-ai/surgical_robotics_challenge/blob/v2.0.0/CHANGELOG.md).

## Timeline

**October 30, 2022:**  Challenge prelaunch

**April 19, 2023:**  Presentation of challenge at [ISMR 2023 Workshop](https://collaborative-robotics.github.io/ismr-2023-workshop.html)

**October 12, 2023:** Registration form activated

**July 12, 2024:** Surgical robotics challenge v2.0.0 released

**January 23, 2025:** First round of online (simulation-based) challenge

**May 2, 2025:** Second (final) round of online (simulation-based) challenge

**Summer 2025:** Physical (in-person) challenge

## Registration

Please register to participate in these challenges. This enables us to inform you about any important updates.

There are no restrictions on who can participate in this challenge. We expect most participants to be part of a team,
so it is only necessary for one person to register the team. If you wish, you can add the names of other participants in the registration form.

[Registration form](https://docs.google.com/forms/d/e/1FAIpQLSdDr5al1koaxZd0Xyuf9S1XG3Mvt-V5wlz3Qm-9CyoWjlJb3w/viewform?usp=sf_link)

## Awards

TBD

## Results


## [System Setup](./system-setup.md)

The challenge is based on the [Asynchronous Multi-Body Framework (AMBF)](https://github.com/WPI-AIM/ambf)
simulator.
Currently, participants will need to install AMBF on a Linux system and clone the surgical robotics challenge assets.
We are investigating a cloud-based solution as an alternative to a local installation.
Note that we are no longer using Docker containers, as in the previous challenge.
Additional details are provided [**here**](./system-setup.md).

## [Submission Instructions]()

TBD

## Challenge Tasks

### Challenge 1: [Grasp needle with right instrument and move to first entry point](./challenge-1.md)

### Challenge 2: [Complete four running sutures using both instruments](./challenge-2.md)

### Contact

Please use the [GitHub Discussions forum](https://github.com/surgical-robotics-ai/surgical_robotics_challenge/discussions) for questions and comments. See the [Community page]() for more information.

To contact the organizers by email: [accelnet-robotics-challenge-admin@googlegroups.com](mailto:accelnet-robotics-challenge-admin@googlegroups.com)

### Acknowledgments

<p><img src="/images/NSF-logo.png" alt="NSF Logo" style="float:left; width:80px; height:80px; margin-right:25px">
Development of this Surgical Robotics Challenge is supported by the United States National Science Foundation (NSF)
via OISE-1927354 and OISE-1927275, <i>AccelNet: International Collaboration to Accelerate Research in Robotic Surgery</i>.</p>
