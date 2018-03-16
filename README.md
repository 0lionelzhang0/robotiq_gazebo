# Robotiq Gazebo

## Setup
1. Uninstall Gazebo2 with
```
sudo apt-get purge gazebo*
```
      Then install Gazebo7 using instructions at http://gazebosim.org/tutorials?tut=install_ubuntu&ver=7.0

2. Download the robotiq package from https://github.com/ros-industrial/robotiq

3. Copy the robotiq folder from this repository to the robotiq folder in your workspace.

4. Build all the files using catkin_make

5. To open gazebo with gripper, run

```
roslaunch robotiq_s_model_articulated_gazebo robotiq.launch
```
   ![alt text](https://github.com/0lionelzhang0/robotiq_gazebo/tree/master/img/gripper.png "Robotiq Gripper in Gazebo")

6. robotiq_pub.py publishes commands to the topic '/left_hand/command'  
Enter positions for A, B, C, and S to command gripper