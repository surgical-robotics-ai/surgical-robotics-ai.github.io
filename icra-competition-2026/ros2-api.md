---
layout: default
---

## ROS2 API

### Robots

All three setups (physical dVRK, AMBF simulation, Isaac Sim simulation) support the same minimal set of ROS 2 topics, using the [CRTK](https://crtk-robotics.readthedocs.io/en/latest/) convention.

The physical dVRK supports the full [documented API](https://dvrk.readthedocs.io/main/pages/development/api/arms.html) for the `PSM1` and `PSM2` namespaces.

The simulated dVRK (AMBF and IsaacSim) supports the following subset of topics in the `PSM1` and `PSM2` namespaces (see above link for documentation):

* `measured_cp`: Measured Cartesian pose, relative to the camera
* `measured_js`: Measured joint state (positions, velocities, effort) for the 6 PSM joints (not including gripper)
* `move_cp`:  Set Cartesian trajectory goal (relative to camera)
* `move_jp`:  Set joint trajectory goal
* `servo_cp`:  Set Cartesian pose goal (relative to camera) for low-level controller
* `servo_jp`:  Set joint position goal for low-level controller (not including gripper)
* `jaw/measured_js`: Measured joint state (positions, velocities, effort) for the gripper
* `jaw/move_jp`:  Set gripper trajectory goal (TBD)
* `jaw/servo_jp`:  Set gripper position goal for low-level controller

### Cameras

The physical (OAK-D-SR) and simulated (AMBF and IsaacSim) stereo camera streams are provided by ROS topics (separate topics for left and right cameras), following the conventional [ROS2 camera configuration](https://docs.ros.org/en/jazzy/p/stereo_image_proc/doc/configuration.html). In particular, the raw left and right camera topics are:

* `stereo/left/image_raw`: raw image stream from left camera
* `stereo/left/camera_info`: calibration parameters for left camera
* `stereo/right/image_raw`: raw image stream from right camera
* `stereo/right/camera_info`: calibration parameters for right camera
