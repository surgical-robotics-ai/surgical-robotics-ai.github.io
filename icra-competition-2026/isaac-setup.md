---
layout: default
---

## IsaacSim Setup

[Isaac Sim Version 5.1.0](https://docs.isaacsim.omniverse.nvidia.com/5.1.0/index.html)
and the corresponding
[Surgical Robotics Challenge Assets (`ros2` branch)](https://github.com/surgical-robotics-ai/isaac-sim-surgical-robotics-challenge/tree/ros2)
are installed on the IsaacSim PC in the competition area.

The simulation environment contains two da Vinci large needle drivers and a pegboard with posts on either side of a large wall. There are two pegs, each with a different color (blue or red).

The virtual stereo camera emulates the OAK-D-SR camera used in [Physical dVRK setup](./dvrk-setup.html). In particular, the stereo baseline is 20 mm, the FOV is 80 deg (H), 55 deg (V), and the resolution is 1280 x 800.

## Human Teleoperation Peg Transfer Challenge

No preparation is necessary -- please come to the competition area and give it a try!

You will use a Quest 3 HMD, with hand controllers, as the interface to control the simulated PSMs.

## Autonomous Peg Transfer Challenge

Competitors for the Autonomous Peg Transfer Challenge should consider one or more of the following options:

### Option 1: Run your algorithm on your own computer

Your computer should be running ROS2 Jazzy and can interface to the IsaacSim computer via a local area connection.

### Option 2: Run your algorithm on the IsaacSim computer

We will create a separate login account for your team, using the account name requested on the registration form.

Following are the specifications for the IsaacSim computer (Alienware laptop):

| CPU | Intel i7 11th gen 2.3GHz 8 cores, 16 threads |
| GPU | RTX 3080 8GB |
| RAM | 32GB |

Packages Installed: ROS2, IsaacSim, Surgical Robotics Challenge Assets

## Offline Development and Testing

If you wish to create the IsaacSim environment on your own computer, please follow the detailed instructions
[here (`ros2` branch)](https://github.com/surgical-robotics-ai/isaac-sim-surgical-robotics-challenge/tree/ros2)

We recommend using ROS2 on Ubuntu 24.04.
