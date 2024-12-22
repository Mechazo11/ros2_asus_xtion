![BSD-3-Clause License](https://img.shields.io/badge/license-BSD--3--Clause-blue.svg)

# ROS 2 ASUS XTION ASSET FOR GAZEBO HARMONIC (OR LATER)

A fork of [ros2_asus_xtion](https://github.com/mgonzs13/ros2_asus_xtion) focused on
integrating Gazebo 8 (Harmonic) or newer's built-in ```rgbd_camera``` plugin for simulated robots.

## Important notes
  
* This package is for simulation only and has not been tested with physical ASUS Xtion cameras.  
* ```asus_xtion_gazebo``` and ```asus_xtion_visualization``` (from the original repo) has been removed to avoid confusion.
* For implementation example, see how this camera asset was used with a simulated Autonomous Mobile Robot (AMR), please check the v0.2 of [clearpath_simulator_harmonic](https://github.com/Mechazo11/clearpath_simulator_harmonic).


**TODO** add picture once placement is fixed correctly

This repo is licensed with BSD-3 license, the same from Miguel's original repository.

## Compatiblity

* ROS 2
  * Jazzy (tested)
* Gazebo
  * Gazebo 8 LTS (Harmonic) 

## Installation

Assuming you workspace is named ```colcon_ws```

```bash
cd ~/colcon_ws/src
git clone -b jazzy_devel --single-branch https://github.com/Mechazo11/ros2_asus_xtion.git
cd ..
colcon build --symlink-install
source ./install_setup.bash
```