# ROS機器人作業系統
本環境使用VirtualBox虛擬機軟體來安裝Ubuntu Linux 20.04

此次開發主題為「...」，目的是提供良好的...

#使用說明:

cd ~/catkin_ws  
catkin_make

1.
開啟終端機(1) RViz
```
roslaunch robot_vacuum_description display.launch
```
開啟終端機(2) 開地圖
```
roslaunch robot_vacuum_description world.launch
```
```
roslaunch robot_vacuum_description navigation.launch   
```

開啟終端機(3)  移動
```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
``` 

建構SLAM
```
roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping   
```
```
rosrun map_server map_saver-f ~/maproom   
```

//清楚描述如何安裝與執行你的ROS套件
```
roslaunch robot_vacuum_description gazebo.launch
```
