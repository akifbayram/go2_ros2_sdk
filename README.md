# go2_ros2_sdk
Unitree go2 ROS 2 drivers are implemented using the go2-WebRTC interface originally designed by @tfoldi (https://github.com/tfoldi/go2-webrtc)

This project enables ROS2 SDK functionality for your Unithree GO2 AIR/PRO

Current state:
1. URDF (Done)
2. Joint states sync (Done) (We have 1sec lag, it will be fixed in near future)
3. IMU sync (Done)
4. Joystick control (Done)
6. Go2 topics info (Done)
7. Foot force sensors info (Done)
8. Camera stream
9. Lidar stream


## Getting started

install ROS 2 (tested on iron)

clone this rep and build it (put go2_interfaces and go2_robot_sdk to src folder of your own ros2_ws repo)
```
git clone https://github.com/abizovnuralem/go2_ros2_sdk.git
pip install -r requirements.txt
colcon build
```

don't forget to put your GO2 in Wifi-mode only and get robot IP
PUT these data into webrtc_driver.py

## Usage
```
source install/setup.bash
ros2 launch go2_robot_sdk robot.launch.py
```

## Topic
![alt text](https://github.com/abizovnuralem/go2_ros2_sdk/blob/master/topics_1.png?raw=true)
