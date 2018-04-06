# Robotiq Gazebo

## Setup
1. Uninstall Gazebo2 with
```
sudo apt-get purge gazebo*
```
2. Install Gazebo7 using instructions at http://gazebosim.org/tutorials?tut=install_ubuntu&ver=7.0

As well as the Gazebo ROS packages
```
sudo apt-get install ros-indigo-gazebo7-ros-pkgs
```

3. Download the robotiq package from https://github.com/ros-industrial/robotiq

4. Copy the robotiq folder from this repository to the robotiq folder in your workspace (replace all files).

5. Build all the files using catkin_make in your workspace

6. To open gazebo with gripper, run

```
roslaunch robotiq_s_model_articulated_gazebo robotiq.launch
```
   ![gripper](https://user-images.githubusercontent.com/36424267/37539067-e6718f6e-290f-11e8-80b1-db5f602a5b40.png)

7. robotiq_pub.py publishes commands to the topic '/left_hand/command'  
Enter positions for A, B, C, and S to command gripper
