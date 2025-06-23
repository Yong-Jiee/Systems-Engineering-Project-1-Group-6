<<<<<<< HEAD
# Systems-Engineering-Project-1-Group-6-
This repository documents my Systems Engineering project at university, using the LIMO mobile robot with ROS1 Melodic to design, build, and test an autonomous navigation system in real-world conditions.
=======
## start the motor driver

```shell
roslaunch limo_bringup limo_start.launch  
# this launch will start motor driver, lidar, imu, robot pose ekf
```

## control Limo by keyboard

first launch the `limo_start.launch` above then launch the keyboard

```shell
# this will publish /cmd_vel topic
roslaunch limo_bringup limo_teletop_keyboard.launch
```

## start the move base for navigation

first launch the `limo_start.launch` above then launch the navigation

```shell
# this will launch the amcl and move_base node
roslaunch limo_bringup limo_navigation.launch
```
<<<<<<< HEAD
>>>>>>> add readme
=======
## build the 2d map

If you want to build the map, you can use `cartographer` , see [the cartographer documents](https://google-cartographer-ros.readthedocs.io/en/latest/)

And then use map_server to save the map, see [map_server](http://wiki.ros.org/map_server)
>>>>>>> change readme
