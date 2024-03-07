# walker_bot

## Overview
This repository contains a simple obstacle avoidance algorithm much like a Roomba robot vacuum cleaner. The turtlebot moves forward until it reaches an obstacle, then rotate in place until the way ahead is clear, then move forward again and repeat.This is demonstrated in gazebo world. 

## Dependencies
* ROS 2 Humble
* Ubuntu 22.04
* Gazebo
* Turtlebot3

## Build Instructions
```
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws/src

git clone https://github.com/NehaMadhekar09/Obstacle_Avoiding_Bot.git

cd ..

rosdep install -i --from-path src --rosdistro humble -y

colcon build 

. install/setup.bash

```
## Run instructions
### 1. Go to directory
```
cd ros2_ws
```
### 2. Source the workspace
```
. install/setup.bash
```
### 3. Run walker node with launch file
```
ros2 launch Obstacle_Avoiding_Bot launch.py
```
