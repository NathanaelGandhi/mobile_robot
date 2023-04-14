# mobile_robot

[Development Log](devlopment_log.md)

## Setup

- Developed in a distrobox (podman) container
  - ros:humble
- apt packages
  - ```sudo apt install -y direnv ros-humble-xacro ros-humble-joint-state-publisher-gui ros-humble-rviz2 ros-humble-gazebo-ros-pkgs```

## Run

- Robot ```ros2 launch mobile_robot rsp.launch.py use_sim_time:=true```
- Joint states publisher gui ```ros2 run joint_state_publisher_gui joint_state_publisher_gui```
- rviz ```rviz2 mobile_robot/conig/view_bot.rviz```
- gazebo ```ros2 launch gazebo_ros gazebo.launch.py```
- spawn robot ```ros2 run gazebo_ros spawn_entity.py -topic robot_description -entity my_robot```
- launch simulation ```ros2 launch mobile_robot launch_sim.launch.py```
  - this loads
    - robot
    - gazebo
    - spawn robot
