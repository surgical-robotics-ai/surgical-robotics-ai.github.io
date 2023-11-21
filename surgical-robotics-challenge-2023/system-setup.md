---
layout: default
---

## System Setup

The challenge is based on the [Asynchronous Multi-Body Framework (AMBF)](https://github.com/WPI-AIM/ambf)
simulator, Version 2.0, along with the
[Surgical Robotics Challenge Assets](https://github.com/surgical-robotics-ai/surgical_robotics_challenge).
To install AMBF and the associated assets (including the launch file) on Linux, follow the detailed instructions
[here](https://github.com/surgical-robotics-ai/surgical_robotics_challenge).

To summarize:

* Install appropriate version of ROS1 (e.g., Noetic on Ubuntu 20.04)
* Install the cv-bridge and image-transport ROS packages:
```bash
apt-get install ros-<version>-cv-bridge ros-<version>-image-transport
```
* Clone the [AMBF repository](https://github.com/WPI-AIM/ambf):
```bash
git clone https://github.com/WPI-AIM/ambf.git
```
* Build the default AMBF branch (`ambf-2.0`) following the [AMBF README](https://github.com/WPI-AIM/ambf/blob/ambf-2.0/README.md)
* Clone the [Surgical Robotics Challenge Assets](https://github.com/surgical-robotics-ai/surgical_robotics_challenge):
```bash
git clone https://github.com/surgical-robotics-ai/surgical_robotics_challenge.git
```
* Install the default branch following the instructions in the [README](https://github.com/surgical-robotics-ai/surgical_robotics_challenge/blob/master/scripts/README.md)
