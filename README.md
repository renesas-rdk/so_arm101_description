# SO ARM101 Description

This package contains the URDF and XACRO description files for the SO ARM101 robotic arm.

## Package Contents

- `urdf/`: URDF and XACRO files describing the robot
- `meshes/`: STL mesh files for visualization
- `launch/`: Launch files for displaying the robot in RViz and Foxglove
- `config/`: Configuration files for display
- `rviz/`: RViz configuration files

## Usage

To visualize the robot in RViz:
```bash
ros2 launch so_arm101_description display_rviz.launch.py
```

To visualize the robot in Foxglove:
```bash
ros2 launch so_arm101_description display_foxglove.launch.py
```

## Robot Specifications

The SO ARM101 is a 6-DOF robotic arm with the following joints:
- shoulder_pan: Base rotation joint
- shoulder_lift: Shoulder elevation joint
- elbow_flex: Elbow flexion joint
- wrist_flex: Wrist flexion joint
- wrist_roll: Wrist rotation joint
- gripper: Gripper joint

## URDF Resource

The original URDF resources for this robot description come from:
https://github.com/TheRobotStudio/SO-ARM100/tree/main

This package has been adapted and converted to follow ROS2 conventions and the xacro macro pattern for better integration with ROS2 robotic systems.