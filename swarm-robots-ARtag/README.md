[README em português](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/README-pt.md)


Description
========================

This scene aims to work with multiple robots in an environment monitored by cameras. Each robot has a glued ARTag, where the identification of the robot's position is done through the “ar_track_alvar" package (http://wiki.ros.org/ar_track_alvar). In this way, the robots do not have odometry, only the cmd_vel topics can be controlled. Each robot has the name referring to the tag id.


Topics
--------------
* Name: /id0_cmd_vel
  - Type: geometry_msgs/Twist.msg
  - description: Topic used to control speeds of robot 0

* Name: /id4_cmd_vel
  - Type: geometry_msgs/Twist.msg
  - description: Topic used to control speeds of robot 4

* Name: /id9_cmd_vel
  - Type: geometry_msgs/Twist.msg
  - description: Topic used to control speeds of robot 9

* Name: /id13_cmd_vel
  - Type: geometry_msgs/Twist.msg
  - description: Topic used to control speeds of robot 13

![](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/swarm-robots-ARtag1.png)
![](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/swarm-robots-ARtag2.png)









