# UR10e Gazebo simulation with Moveit

clone the ur_description package using the following command 
```
git clone https://github.com/ros-industrial/universal_robot.git
```
This repository contains the packages for ur robots description, gazebo model and moveit confirgurations. 

To bring up the simulated robot in Gazebo, run:
```
roslaunch ur_gazebo ur10e_bringup.launch
```
MoveIt! with a simulated robot Again, you can use MoveIt! to control the simulated robot. For setting up the MoveIt! nodes to allow motion planning run:
```
roslaunch ur10e_moveit_config moveit_planning_execution.launch sim:=true
```
For starting up RViz with a configuration including the MoveIt! Motion Planning plugin run:
```
roslaunch ur10e_moveit_config moveit_rviz.launch
```


