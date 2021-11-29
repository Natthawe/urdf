ros2 pkg create --build-type ament_cmake <you_pkg_name>

ros2 pkg create --build-type ament_python <you_pkg_name> --dependencies rclpy <pkg_name>

rosdep install -i --from-path src --rosdistro galactic -y

colcon build --symlink-install

colcon build --packages-select <pkg_name>

. install/setup.bash

ros2 doctor

rosdep install -y -r -q --from-paths src --ignore-src --rosdistro

sudo apt-get install python3-rosdep -y sudo rosdep init rosdep update rosdep install -i --from-path src --rosdistro $ROS_DISTRO -y

sudo apt install ros-galactic-xacro

sudo apt install ros-galactic-joint-state-publisher-gui