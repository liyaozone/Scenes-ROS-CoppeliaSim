[README em português](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/README-pt.md)


Description
========================

This scene aims to bring a robot that does not have odometry (encoder on its wheels). The Robot is equipped with a LaserScan sensor and an RGB camera. The goal is to use the scene to study localization techniques that do not involve the use of encoder odometry, such as hector_slam.No TF is created to simulate the situation where the robot only navigates through the Lidar, without the need for base_link and other frames.


Topics
--------------
* Name: /cmd_vel
  - Type: geometry_msgs/Twist.msg
  - description: The topic used to control the speeds of the robot.

* Name: /scan
  - Type: sensor_msgs/LaserScan
  - Frame: Lidar
  - description: The topic is containing a Lidar sensor information,  in laser Scan format.

* Name: /usb_cam/camera_info
  - Type: sensor_msgs/CameraInfo
  - Frame: "usb_cam"
  - description: The topic contains the image information to be published in the "/usb_cam/image_raw" topic.

* Name: /usb_cam/image_raw
  - Type: sensor_msgs/Image
  - Frame: "usb_cam"
  - description: The topic contains the image in the RGB format captured by the vision sensor.

![](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/robot-without-odometry_1.png)
![](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/robot-without-odometry_2.png)









