本文档对与TB2+RPlidar软件安装使用说明

1.参考教程安装rplidar驱动,网页链接:https://github.com/robopeak/rplidar_ros


2.安装Turtlebot的ROS包


3.将文件夹中的文件,放到相应的Turtlebot的ROS包的文件夹下(一定要对应相应的路径)


4.连接TB2底座,连接rplidar


5.输入环境变量, echo "export TURTLEBOT_3D_SENSOR=rplidar" >> ~/.bashrc && source ~/.bashrc


5.启动Turtlebot, roslaunch turtlebot_bringup minimal.launch


6.启动rplidar, roslaunch rplidar_ros rplidar.launch


7.gmapping+move_base, roslaunch turtlebot_navigation rplidar_gmapping.launch


8.map_serve+gmapping+move_base, roslaunch turtlebot_navigation rplidar_amcl.launch

