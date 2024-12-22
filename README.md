# Turtlebot Navigation using Nav2 SLAM

## Description:
This project was just to test out Turtlebot navifation using the Nav2 in ROS2 Galactic environment.

## Dependencies:
It is assumed that the ROS2 Galactic is already installed and setup in your system. Is it's not setup, navigate to [ROS Documentation](https://docs.ros.org/en/galactic/Installation.html) for installing ROS2.
You also need navifation2, nav2-bringup and turtlebot3 packages, which can be installed using the below commands.
<code>sudo apt install ros-galactic-navigation2</code>
<code>sudo apt install ros-galactic-nav2-bringup</code>
<code>sudo apt install ros-galactic-turtlebot3'*'</code>

## Build the package:
Create a folder using the below command

<code>mkdir ros_ws/src</code>

navigate to the src folder 

<code>cd ros_ws/src</code>

Copy this package turtlebot3_project3 into the src folder and navigate outside src.

<code>cd..</code>

Build the turtlebot3_project3 package using the below command.

<code>colcon build --packages-select turtlebot3_project3</code>

Source the file using the below command

<code>source install/setup.bash</code>

## Usage:
To run the package run the below commands:

<code>ros2 launch turtlebot3_project3 turtlebot3_world.launch.py</code>

<code>ros2 launch turtlebot3_navigation2 navigation2.launch.py use_sim_time:=True map:='src/turtlebot3_project3/map∕my_map.yaml'</code>

<code>ros2 run turtlebot3_project3 turtlebot3_navigation</code>
