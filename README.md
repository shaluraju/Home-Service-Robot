# Home Service Robot
## Objective
This is the final project of **_Udacity Robotics Software Engineer_** Nano Degree Program which applies ***SLAM and Navigation*** on mobile robot. The goal of this project was to design a robot's environment in gazebo and program the home-service robot that will map it's environment and autonomously navigate to pre-specified pickup and drop-off locations(_Performing Delivery_). For this one needed to:
- Design robot's environment with the Building Editor in Gazebo.
- Teleoperate the robot and manually test SLAM.

- Write a pick_objects node that commands the robot to move to the desired pickup and drop off zones.
- Write an add_markers node that subscribes to the robot odometry and publishes pick-up and drop-off markers to rviz.
- modify pick_objects node and add_markers node to establish communication between them, to complete desired home service robot implementation

## Video of a Mobile Robot delevering a Square Box 


![ezgif com-gif-maker](https://user-images.githubusercontent.com/67613439/125275120-43c54500-e32c-11eb-8349-713900f530ae.gif)

### Project Structure
This directory represents the main project's **src** folder structure with following contents

- images - folder with images and videos for this report
- add_markers - add marker C++ node
- config - folder with configuration file to specify pick-up and drop-off locations
- map - map and gazebo world files
- pick_objects - pick-objects C++ node
- rvizConfig - folder with rViz configurations used with some launch scripts
- scripts - shell scripts
  - add_marker.sh - script for testing add_marker concept with add_markers.cpp
  - home_service.sh - main script for the home-service-robot
  - pick_objects.sh - script for testing pick_objects concept with pick_objects.cpp
  - test_navigation.sh - script for testing navigation
  -test_slam.sh - script for performing SLAM and preparing map
- slam_gmapping - official ROS package with gmapping_demo.launch file
- turtlebot - official ROS package with keyboard_teleop.launch file
- turtlebot_interactions - official ROS package with view_navigation.launch file
turtlebot_simulator - official ROS package with turtlebot_world.launch file

### Configuration
- Ubuntu 16.04 OS with default make (>=4.1) and g++/gcc (>=5.4) packages
- Gazebo >= 7.0
- ROS Kinetic
- Following ROS packages were used and the process of obtaining them is detailed below:
  - gmapping
  - turtlebot_teleop
  - turtlebot_rviz_launchers
  - turtlebot_gazebo

### Gazebo Environment
![environment](https://user-images.githubusercontent.com/67613439/125280102-5478b980-e332-11eb-9660-285a5f9ec382.png)

