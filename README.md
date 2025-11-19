# yahboom-7-DOF-ARM-ROS2-TEST
may work or not work it worked for me on my jetson orin nano.


# JetCobot 7-DOF ROS2 Package 🤖

ROS2 package for controlling the **Yahboom JetCobot 7 DOF collaborative robotic arm**  
with Jetson Nano / Jetson Orin and ROS2 (tested with Humble / Foxy style layout).

> **Note:** This repo provides a *clean structure and example nodes*.  
> You’ll still need to plug in Yahboom's official SDK / drivers for real hardware comms.

---

## Features

- 7-DOF joint control interface
- `arm_driver.py` – low-level driver node (placeholder for Yahboom SDK)
- `arm_controller.py` – high-level controller that publishes joint commands
- `teleop_keyboard.py` – keyboard-based joint teleoperation
- `preset_motions.py` – example motion sequences
- Launch files to bring up the whole stack

---

## Installation

```bash
# In your ROS2 workspace
cd ~/ros2_ws/src
git clone https://github.com/<your-username>/ros2-jetcobot-arm.git
cd ..
colcon build
source install/setup.bash
