# Development Log

## 20230414

- setup a distrobox with ros:humble
- installed direnv ```sudo apt install direnv```
- created a workspace with a .envrc linking to humble
- followed <https://articulatedrobotics.xyz/mobile-robot-1-project-overview/>
  - created a repo from the template: <https://github.com/joshnewans/my_bot>
  - cloned to my git folder
  - symlinked to my ros workspace
  - replaced all references to ```my_bot``` with ```mobile_robot```
  - updated descriptions in the package.xml
- updated ros dependencies to get armet_cmake
- build the workspace ```colcon build --symlink-install```
- install xacro and joint_state_publisher_gui
  - ```sudo apt install ros-humble-xacro```
  - ```sudo apt install ros-humble-joint-state-publisher-gui```
- create robot_core.xacro
- installed rviz ```sudo apt install ros-humble-rviz2```
- get wheels to show in rviz ```ros2 run joint_state_publisher_gui joint_state_publisher_gui```
- add inertial macros to robot description
- saved the rviz config to ```mobile_robot/config/view_bot.rviz```
