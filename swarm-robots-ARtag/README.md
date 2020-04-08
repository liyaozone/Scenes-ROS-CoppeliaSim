[README em português](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/README-pt.md)


Description
=================================

This package aims to store scenes used in the CoppeliaSim Edu simulator (https://coppeliarobotics.com/download) designed to work together with the ROS (Robot Operating System) through the ROS Interface API ((https://www.coppeliarobotics.com/helpFiles/en/rosInterf.htm). In this way, the scenes presented in this package can read and send information to ROS.

Configuration of the system used
--------------------------------

* Ubuntu 18.04.4 (http://releases.ubuntu.com/18.04.4/)
* ROS Melodic (http://wiki.ros.org/melodic/Installation/Ubuntu)



Installing CoppeliaSim Edu on Ubuntu 18.04
--------------------------------
* Download the desired version at https://coppeliarobotics.com/ubuntuVersions
  - For the version "CoppeliaSim_Edu_V4_0_0_Ubuntu18_04" follow the steps below:

```
$ cd ~/ 
$ wget https://coppeliarobotics.com/files/CoppeliaSim_Edu_V4_0_0_Ubuntu18_04.tar.xz 
$ tar -xf CoppeliaSim_Edu_V4_0_0_Ubuntu18_04.tar.xz 
```

* You need to add the ROSInterface library in the main compiledRosPlugins folder. The library was already compiled into the "compiledRosPlugins" folder. Let's copy the file “libsimExtROSInterface.so”.

```
$ cd ~/CoppeliaSim_Edu_V4_0_0_Ubuntu18_04/
$ cp compiledRosPlugins/libsimExtROSInterface.so libsimExtROSInterface.so
```

Run:
-------------------------------

* To run CoppeliaSim, just run the file “coppeliaSim.sh”. You must have **roscore** initialized.

```
$ roscore
$ cd ~/CoppeliaSim_Edu_V4_0_0_Ubuntu18_04/
$ ./coppeliaSim.sh
```

* Check in the terminal if the following message appears
  - Plugin 'ROSInterface': load succeeded.

![](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/img1.png)
![alt text](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/img2.png)
![alt text](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/img3.png)
![alt text](https://github.com/marco-teixeira/Scenes-ROS-CoppeliaSim/blob/master/images/img4.png)







