README.md
 
ROS2 Medical Autonomous Delivery Robot Project
 
Overview
 
This project is based on ROS2 Humble for OriginCar mobile chassis, developed for college intelligent robot competition. It realizes SLAM mapping, autonomous navigation, LiDAR obstacle avoidance and multi-point medical material delivery.
 
The code consists of two parts:  origincar_base  (hardware driver) and  ros2_ws  (navigation & task logic).
 
Directory
 
- origincar_base: Chassis motor control, odometer and basic launch files.
- ros2_ws: Navigation workspace, including map resources, Python/C++ nodes, launch files and config params.
 
Main Functions
 
1. LiDAR driver & chassis motion control
2. Real-time SLAM mapping
3. AMCL localization, global & local path planning
4. Multi-waypoint cyclic delivery task
5. Dynamic obstacle avoidance
 
Build & Run
 
bash
  
cd ros2_ws
colcon build
source install/setup.bash
ros2 launch racecar nav10_map.launch.py
