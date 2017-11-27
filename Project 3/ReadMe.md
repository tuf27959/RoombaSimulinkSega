
# RoombaROS
**Sega Diallo Temple University School of Engineering**

**Advisor Dr Li Bai**
```
This project is to create a ROS Publisher and Subscriber for the Roomba. 
The Publisher is for the Range Sensor State which gives the available six sensors status. 
The Subscriber is for the Left and Right Wheel Control. 
For the project the Roomba is connected via USB serial cable.
```
**Pre-requisits**
1. For basic information about the Raspberry pi you can refer to the following link(https://www.raspberrypi.org).
2. Ubuntu is a requirement for this project, the installation instruction can be found at the following link(https://wiki.ubuntu.com/ARM/RaspberryPi).
3. The intructions on how to install ROS/Kinect can be found at the following link(http://wiki.ros.org/Installation/UbuntuARM)
4. Finally the libraries to control the Roomba can be found at the following link(https://pypi.python.org/pypi/pycreate2/0.7.3).
5. A good book for reference about ROS is (O'REILLY: Programming Robots with ROS)

**USING ROS**
In order to use ROS first we have to create a workspace by typing the following command lines;
```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
catkin_init_workspace
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```
Then create a package into the workspace
```
cd ~/catkin_ws/src
catkin_create_pkg roomba rospy
```
Then Go into Roomba source folder directory to add the python scripts
```
cd ~/catkin_ws/src/roomba/src
```
Paste the wheel and sensor scripts by typing the following line:
```
git clone https://github.com/tuf27959/RoombaSimulinkSega/tree/master/Project%203
```
Then go back to Catkin_ws
```
cd ~/catkin_ws
```
Type the bash Command
```
source devel/setup.bash
```
We are all set the next steps are to open two secondary terminal windows one for the Subscriber and 
and one for the Publisher. The main terminal window is call the Master.
