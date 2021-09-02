# ROS-Robot-Description-Package
This package contains the robot description using URDF/XACRO including the gazebo laser-scanner and the gazebo_ros_control-plugin.
## Launch files
- show_robot_rviz.launch: Uses the joint_state_publisher to publish and control fake joint states and the robot_state_publisher to combine those into one transform. Visualizes the final robot in Rviz.
- show_robot_gazebo.launch: Launches Gazebo with a specified .world file and loads the robot model.

![Screenshot from 2021-09-02 19-41-08](https://user-images.githubusercontent.com/49548379/131893653-b58ed245-1241-4717-bff2-85ec9479cfa5.png)

- show_robot_gazebo_rviz.launch: Launches Gazebo with a specified .world file and loads the robot model. Furthermore the gazebo_ros_controllers are loaded to publish the actual joint states (JointStateController) and control the robot (DiffDriveController). The Joint states are combined using the robot_state_publisher. This allows to display the robot in Rviz aswell. The robot can be controlled by utilizing the rqt_robot_steering package.

![gazebo_rviz_gazebo](https://user-images.githubusercontent.com/49548379/131893689-a464871d-3106-445e-b206-7296963964e0.png)
![gazebo_rviz_rviz](https://user-images.githubusercontent.com/49548379/131893699-49f06f6b-9d83-47ca-bb23-7313ad400f31.png)

