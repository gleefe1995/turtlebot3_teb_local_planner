# turtlebot3_teb_local_planner
teb_local_planner in turtlebot3 ubuntu 18.04 melodic

cartographer로 실행한 결과 입니다.
gmapping으로도 실행 가능합니다. 
turtlebot3 에서 roslaunch turtlebot3_bringup turtlebot3_robot.launch실행 

or 

가제보에서 실행하려면
roslaunch turtlebot3_gazebo turtlebot3_world.launch 실행후 

roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=cartographer configuration_basename:=turtlebot3_lds_2d_gazebo.lua

로 slam 실행.

add-bytopic 에서 teb_planner에서 global, local planner- 각각 path 추가 후 색깔 다르게 해주시고 
navigation goal을 찍으면 path가 뜹니다. 

rosrun rqt_reconfigure rqt_reconfigure 로 여러 parameter 바꿔보면서 실행 가능.


cartographer teb_local_planner turtlebot3 gazebo simulation
![Screenshot from 2020-09-03 00-50-54](https://user-images.githubusercontent.com/67038853/92017270-7c9ca100-ed8e-11ea-90a7-e79bdb1011b2.png)

