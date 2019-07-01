# gazebo_ros_env

## Run gazebo with ros

### Prepare

#### At the very first time to use this gazebo_ros_controller, please follow the instructions below.
1. Build up a ros environment (kinetic) well on your Ubuntu 16.04. You can build up with docker (Please check the README.md in ./catkin_ws/src/README.md in this repo.). Or you can also use images created by ROS fundation on Docker_Hub.

2. Next, create a workspace.
- `cd ~` 
- `mkdir catkin_ws && cd catkin_ws`

3. Clone the whole repo into your new workspace catkin_ws.
- `git clone https://github.com/lluma/gazebo_ros_env.git`

4. Finally, run make with the workspace. 
- `source /opt/ros/kinetic/setup.bash && catkin_make`

#### If you've already had the environment to ROS, please feel free to follow the instructions below.  
1. Go to the workspace.
- `cd ~/catkin_ws`.

2. Then ensure that your environment with base is sourced. If not, please do `source ~/catkin_ws/devel/setup.bash`. 

### Run some tests.
#### Run the gazebo with our testing launch files.
- Try `roslaunch tm_gazebo testing_tm700.launch`.

#### Some error reduction.
If you have any error when running the above commands, please try `sudo apt-get update && sudo apt-get upgrade` first.
