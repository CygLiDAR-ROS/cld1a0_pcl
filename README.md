# cyglidar_d1
cyglidar_d1 is a ROS package, which is designed to visualize 2D/3D distance dataset in real-time.
For more details in CygLiDAR, please visit http://www.cygbot.com

## How to use this package

### Preparation
1) Clone this project to your catkin's workspace
2) Run catkin_make

### Set-Up
Install the udev rule
```bash
roscd cyglidar_d1
cd scripts
chmod +x create_udev_rules.sh
./create_udev_rules.sh
```

### Parameters
In cyglidar.launch, the version number of datasets can be switched 0(2D) and 1(3D) as below:

2D)
<h1 align="left">
  <img src="screenshots/param_2d.png" width="600"/>
</h1>

3D)
<h1 align="left">
  <img src="screenshots/param_3d.png" width="600"/>
</h1>

### Run
```bash
roslaunch cyglidar_d1 cyglidar.launch
```

### Note
In Rviz, the fixed frame and the topic for Point Cloud are respectively equivalent to the following:

##### Fixed Frame
```bash
/laser_link
```

##### Topic
```bash
/scan
```
