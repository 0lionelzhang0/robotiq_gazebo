# Robotiq Gazebo

## Setup
1. Uninstall Gazebo2 with
```
sudo apt-get purge gazebo*
```
   Then install Gazebo7 using instructions at http://gazebosim.org/tutorials?tut=install_ubuntu&ver=7.0

2. Download the robotiq package from https://github.com/ros-industrial/robotiq

3. Copy the robotiq folder from this repository to the robotiq folder in your workspace (replace all files).

4. Build all the files using catkin_make in your workspace

5. To open gazebo with gripper, run

```
roslaunch robotiq_s_model_articulated_gazebo robotiq.launch
```
   ![gripper](https://user-images.githubusercontent.com/36424267/37539067-e6718f6e-290f-11e8-80b1-db5f602a5b40.png)

6. robotiq_pub.py publishes commands to the topic '/left_hand/command'  
Enter positions for A, B, C, and S to command gripper
