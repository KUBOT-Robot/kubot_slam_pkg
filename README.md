# kubot_slam_pkg

[![Apache-2.0 License](https://img.shields.io/badge/license-Apache2.0-purple)](https://opensource.org/licenses/Apache-2.0).
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Platform Badge](https://img.shields.io/badge/platform-ROS_Melodic-blue.svg)](http://wiki.ros.org/melodic)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![version](https://img.shields.io/badge/version-1.0.1-green)](https://robot.shayangye.com/robots/59)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![robot](https://img.shields.io/badge/robot-KUBOT-orange)](http://www.shayangye.com/)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

# Introduction

This is the [Simultaneous Localization and Mapping (SLAM)](https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping) package for the KUBOT robot. It includes Vehicle control calibration, [Move_base](http://wiki.ros.org/move_base), Lidars, 2D SLAM, 3D SLAM and [Navigation](http://wiki.ros.org/navigation), etc.

# Repository Contents
- [x] [kubot_control](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.1-kubot_control)
	- [x] teleop_keyboard_control.launch
	- [x] navigation_multi_demo.launch
	- [x] usb_camera.launch
	- [x] calibrate_linear.py
	- [x] calibrate_angular.py
- [x] [kubot_lidar](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.2-kubot_lidar)
	- [ ] lidars
	- [x] lidar_filter.launch
   - [x] ira_lidar.launch
- [ ] kubot_3dsensor
	- [ ] 3dsensor.launch
- [x] [kubot_slam_2d](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.3-kubot_slam_2d)
	- [x] gmapping_simulation.launch
	- [x] gmapping_with_robot.launch
	- [x] hector_mapping.launch
	- [x] hector_mapping_without_odom.launch
	- [x] catographer.launch
	- [x] catographer_with_odom.launch
	- [x] karto_slam.launch
	- [x] view_cartographer.launch
- [ ] [kubot_slam_3d](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.5-kubot_slam_3d)
	- [ ] rtabmap.launch
- [x] [kubot_navigation](https://github.com/KUBOT-Robot/kubot_ros/wiki/4.4-kubot_navigation)
	- [x] move_base
	- [x] amcl
	- [ ] rgbd_move_base
	- [ ] rgbd_amcl
	- [ ] maps
	- [x] save_map.launch
	- [x] navigation.launch
	- [x] view_rviz.launch
- [ ] third_party_pkg

# Install

```sh
cd ~/kubot_ros/ros_ws/src
git clone https://github.com/KUBOT-Robot/kubot_slam_pkg.git -b melodic-devel
cd ..
catkin_make
source ~/.bashrc
```