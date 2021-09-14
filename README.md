# kubot_slam_pkg

[![Apache-2.0 License](https://img.shields.io/badge/license-Apache2.0-purple)](https://opensource.org/licenses/Apache-2.0).
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Platform Badge](https://img.shields.io/badge/platform-ROS_Noetic-blue.svg)](http://wiki.ros.org/noetic)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![version](https://img.shields.io/badge/version-1.0.1-green)](https://robot.shayangye.com/robots/59)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![robot](https://img.shields.io/badge/robot-KUBOT-orange)](http://www.shayangye.com/)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

# Introduction

This is the [Simultaneous Localization and Mapping (SLAM)](https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping) package for the KUBOT robot. It includes Vehicle control calibration, [Move_base](http://wiki.ros.org/move_base), Lidars, 2D SLAM, 3D SLAM and [Navigation](http://wiki.ros.org/navigation), etc.

# Repository Contents
- [ ] [kubot_control](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.1-kubot_control)
	- [ ] teleop_keyboard_control.launch
	- [ ] navigation_multi_demo.launch
	- [ ] usb_camera.launch
	- [ ] calibrate_linear.py
	- [ ] calibrate_angular.py
- [ ] [kubot_lidar](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.2-kubot_lidar)
	- [ ] lidars
	- [ ] lidar_filter.launch
    - [ ] ira_lidar.launch
- [ ] kubot_3dsensor
	- [ ] 3dsensor.launch
- [ ] [kubot_slam_2d](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.3-kubot_slam_2d)
	- [ ] gmapping_simulation.launch
	- [ ] gmapping_with_robot.launch
	- [ ] hector_mapping.launch
	- [ ] hector_mapping_without_odom.launch
	- [ ] catographer.launch
	- [ ] catographer_with_odom.launch
	- [ ] karto_slam.launch
	- [ ] view_cartographer.launch
- [ ] [kubot_slam_3d](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.5-kubot_slam_3d)
	- [ ] rtabmap.launch
- [ ] [kubot_navigation](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.4-kubot_navigation)
	- [ ] move_base
	- [ ] amcl
	- [ ] rgbd_move_base
	- [ ] rgbd_amcl
	- [ ] maps
	- [ ] save_map.launch
	- [ ] navigation.launch
	- [ ] view_rviz.launch
- [ ] third_party_pkg

# Install

```sh
cd ~/kubot_ros/ros_ws/src
git clone https://github.com/KUBOT-Robot/kubot_slam_pkg.git -b noetic-devel
cd ..
catkin_make
source ~/.bashrc
```