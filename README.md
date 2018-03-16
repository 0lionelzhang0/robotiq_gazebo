# Robotiq Gazebo

## Setup

1. Download the robotiq package from https://github.com/ros-industrial/robotiq

2. Copy the robotiq folder in this repository into the robotiq folder in your workspace.

3. Build all the files using catkin_make



4. To open gazebo with gripper, run

```
roslaunch robotiq_s_model_articulated_gazebo robotiq.launch
```

5. robotiq_pub.py publishes commands to the topic '/left_hand/command'
Enter positions for A, B, C, and S to command gripper