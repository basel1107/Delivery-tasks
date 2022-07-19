# Delivery-tasks
Installation
sudo apt update
Now pick how much of ROS you would like to install.

Desktop-Full Install: (Recommended) : Everything in Desktop plus 2D/3D simulators and 2D/3D perception packages

sudo apt install ros-noetic-desktop-full
Desktop Install: Everything in ROS-Base plus tools like rqt and rviz

sudo apt install ros-noetic-desktop
ROS-Base: (Bare Bones) ROS packaging, build, and communication libraries. No GUI tools.

sudo apt install ros-noetic-ros-base
There are even more packages available in ROS. You can always install a specific package directly.

sudo apt install ros-noetic-PACKAGE
e.g.

sudo apt install ros-noetic-slam-gmapping
Environment setup
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc

source ~/.bashrc
if you use zsh

echo "source /opt/ros/noetic/setup.zsh" >> ~/.zshrc
source ~/.zshrc
Dependencies for building packages
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
Initialize rosdep
sudo apt install python3-rosdep
With the following, you can initialize rosdep.

sudo rosdep init
rosdep update

