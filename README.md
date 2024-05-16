# 4 Wheel Differential Drive Robot in ROS2 foxy. All files including Xacro, Gazebo & Launch are in repo.

Create ws_mobile directory
```
mkdir ws_mobile
```

Clone the repository
```
git clone https://github.com/SaadRana17/4-Wheel-Differential-Drive-Robot.git

```

Going In folder
```
cd 4-Wheel-Differential-Drive-Robot

```


Source the environment
```
source /opt/ros/foxy/setup.bash

```

build the workspace. Make sure you're in ws_mobile folder before building
```
colcon build

```

Source the workspace
```
source ~/ws_mobile/install/setup.bash

```

Run the launch file. This will open the 4-wheel-robot model in gazebo
```
ros2 launch mobile_robot gazebo_model.launch.py

```
![](https://github.com/SaadRana17/4-Wheel-Differential-Drive-Robot/blob/main/1_ws.gif)
![](https://github.com/SaadRana17/4-Wheel-Differential-Drive-Robot/blob/main/2_ws.gif)

Open new terminal and source the environment variable again
```
source /opt/ros/foxy/setup.bash

```

Start the teleop to operate robot from keyboard. Make sure teleop terminal window is open over on gazebo else robot won't move.
```
ros2 run teleop_twist_keyboard teleop_twist_keyboard

```

![](https://github.com/SaadRana17/4-Wheel-Differential-Drive-Robot/blob/main/3_ws.gif)
![](https://github.com/SaadRana17/4-Wheel-Differential-Drive-Robot/blob/main/4_ws.gif)

