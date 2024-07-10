## Run commands
```
# ROS
  # Underdelay
  source /opt/ros/humble/setup.zsh # ROS2 system install & Default environment
  source ~/ros2_ws/install/setup.zsh # ROS workspace Preferences & Use

  
  source /usr/share/colcon_argcomplete/hook/colcon-argcomplete.zsh
  source /usr/share/vcstool-completion/vcs.zsh
  source /usr/share/colcon_cd/function/colcon_cd.sh
  export _colcon_cd_root=~/ros2_ws


  export ROS_DOMAIN_ID=0
  export ROS_NAMESPACE=robot1


  # DDS
  export RMW_IMPLEMENTATION=rmw_fastrtps_cpp
  # export RMW_IMPLEMENTATION=rmw_connext_cpp
  # export RMW_IMPLEMENTATION=rmw_cyclonedds_cpp
  # export RMW_IMPLEMENTATION=rmw_gurumdds_cpp


  # export RCUTILS_CONSOLE_OUTPUT_FORMAT='[{serverity} {time}] [{name}] {message} ({function}() at {file_name}:{line_number})'
  export RCUTILS_CONSOLE_OUTPUT_FORMAT='[{serverity}]: {message}'
  export RCUTILS_COLORIZED_OUTPUT=1
  export RCUTILS_LOGGING_USE_STDOUT=0
  export RCUTILS_LOGGING_BUFFERED_STREAM=0


  alias cw='cd ~/ros2_ws'
  alias cs='cd ~/ros2_ws/src'
  alias ccd='colcon_cd'


  alias cb='cd ~~/ros2_ws && colcon build --symlink-install'
  alias cbs='colcon build --symlink-install'
  alias cbp='colcon build --symlink-install --packages-select'
  alias cbu='colcon build --symlink-install --packages-up-to'
  alias ct='colcon test'
  alias ctp='colcon test --packages-select'
  alias ctr='colcon test-result'


  alias rt='ros2 topric list'
  alias re='ros2 topic echo'
  alias rn='ros2 node list'

  
  alias killgazebo='killall -9 gazebo & killall -9 gzserver & killall -9 gzclient'


  alias af='ament_flask8'
  alias ac='ament_cpplint'


  alias testpub='ros2 run demo_nodes_cpp talker'
  alias testsub='ros2 run demo_nodes_cpp listener'
  alias testpubimg='ros2 run image_tools cam2image'
  alias testsubimg='ros2 run image_tools showimage'
```
