# -In-ROS2-Humble-to-perform-simulation-mapping-and-navigation
学习了鱼香ROS的文档，我在ROS2 humble版本中进行二轮差速车的仿真，建图，导航。
  
在src文件中获取cartographer,cartographer_ros,navigation2
源码安装
git clone https://ghproxy.com/https://github.com/ros2/cartographer.git -b ros2
git clone https://ghproxy.com/https://github.com/ros2/cartographer_ros.git -b ros2
git clone https://ghproxy.com/https://github.com/ros-planning/navigation2.git -b humble
  
https://ghproxy.com如果你有代理，这部分你可以不需要

此时你的文件已经齐全了，如果你有相关配置，可以在/src文件下打开终端
colcon build

然后
source install/setup.bash
ros2 launch fishbot_description gazebo.launch.py

source install/setup.bash
ros2 launch fishbot_navigation2 navigation2.launch.py
通过这两个命令行，你可以运行自主导航

source install/setup.bash
ros2 launch fishbot_description gazebo.launch.py

source install/setup.bash 
ros2 launch fishbot_cartographer cartographer.launch.py
这两个命令行是建图

相关的我学习做这些文件的过程，我会在我的个人网站上发布：https://crp30.top/docs/category/ros2%E5%AD%A6%E4%B9%A0%E7%AC%94%E8%AE%B0
