[README em português](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/README-pt.md)


Description
========================

This scene aims to bring a robot that have odometry. The Robot is equipped with a LaserScan sensor and an RGB camera. The robot also has the Tf (http://wiki.ros.org/tf), which connects all components of the robot, connecting the cameras to base_link, and base_link to the Odom frame (robot starting point). 


Tf
-----------------
![](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/robot-tf.png)




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









